---
name: Create and lock a Distributed Validator cluster
description: Accept terms, propose a cluster definition, collect operator acceptances, and publish the signed cluster lock via the Obol API.
api: openapi/obol-openapi-original.json
operations:
  - TermsAndConditionsController_signTermsAndConditions_v1
  - DefinitionController_postClusterDefinition_v1
  - DefinitionController_updateClusterDefinition_v1
  - LockController_postClusterLock[1]_v1
  - LockController_getClusterLock[1]_v1
---

# Create and lock a Distributed Validator cluster

Use the Obol API (`https://api.obol.tech`, `/v1/...`) to bootstrap a Distributed Validator (DV) cluster.

## Auth & conventions
- Write endpoints require an `Authorization: Bearer <JWT>` header (see `authentication/obol-authentication.yml`). The JWT is an EIP-712 signature from the operator's wallet, as handled by `@obolnetwork/obol-sdk`.
- Errors return `application/json` (see `errors/obol-problem-types.yml`). No idempotency key is supported — do not blindly retry POSTs.

## Steps
1. **Accept the latest terms** with `TermsAndConditionsController_signTermsAndConditions_v1` (`POST /v1/termsAndConditions`). This is required before proposing a definition.
2. **Propose the cluster definition** with `DefinitionController_postClusterDefinition_v1` (`POST /v1/definition`). Returns the `configHash`.
3. **Each operator accepts** the definition with `DefinitionController_updateClusterDefinition_v1` (`PUT /v1/definition/{configHash}`) — a `409` means the operator already accepted.
4. After the distributed key generation (DKG) ceremony, **publish the cluster lock** with `LockController_postClusterLock[1]_v1` (`POST /v1/lock`). Returns the `lockHash`.
5. **Confirm** with `LockController_getClusterLock[1]_v1` (`GET /v1/lock/{lockHash}`).
