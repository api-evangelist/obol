---
name: Inspect a Distributed Validator cluster
description: Look up a cluster lock and read its validator states, peer scores, and effectiveness via the Obol API.
api: openapi/obol-openapi-original.json
operations:
  - LockController_getClusterLock[1]_v1
  - StateController_getDistributedValidatorStatesByLockHash_v1
  - LockController_getAveragePeerScores[1]_v1
  - EffectivenessController_getClusterLock_v1
---

# Inspect a Distributed Validator cluster

Read the health and state of an existing DV cluster via the Obol API (`https://api.obol.tech`). All of these endpoints are public reads.

## Steps
1. **Fetch the cluster lock** with `LockController_getClusterLock[1]_v1` (`GET /v1/lock/{lockHash}`) to get the operators, validators, and configuration.
2. **Read validator states** with `StateController_getDistributedValidatorStatesByLockHash_v1` (`GET /v1/state/{lockHash}`).
3. **Read average peer scores** for the operators with `LockController_getAveragePeerScores[1]_v1` (`GET /v1/lock/{lockHash}/peer-scores`).
4. **Read cluster effectiveness** with `EffectivenessController_getClusterLock_v1` (`GET /v1/effectiveness/{lockHash}`).

## Notes
- Errors return `application/json` (see `errors/obol-problem-types.yml`); a `404` means no cluster is registered for that `lockHash`.
