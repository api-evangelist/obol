---
name: Exit a Distributed Validator
description: Submit partial signed exit messages for a DV cluster and track exit status through the Obol API.
api: openapi/obol-openapi-original.json
operations:
  - ExitController_postPartialExit[1]_v1
  - ExitController_getClusterExitStatus[1]_v1
  - ExitController_getClusterExitStatusSummary[1]_v1
  - ExitController_getClusterExit[1]_v1
---

# Exit a Distributed Validator

Coordinate a threshold exit of a Distributed Validator (DV) cluster via the Obol API (`https://api.obol.tech`).

## Auth & conventions
- `ExitController_getClusterExit[1]_v1` requires an `Authorization: Bearer <JWT>` header; the status endpoints are public.
- Errors return `application/json` (see `errors/obol-problem-types.yml`). A `409` on a partial-exit push means that share was already submitted.

## Steps
1. **Each operator pushes its partial signed exit** with `ExitController_postPartialExit[1]_v1` (`POST /v1/exp/partial_exits/{lockHash}`).
2. **Poll the exit status** with `ExitController_getClusterExitStatus[1]_v1` (`GET /v1/exp/exit/status/{lockHash}`) or the roll-up `ExitController_getClusterExitStatusSummary[1]_v1` (`GET /v1/exp/exit/status/summary/{lockHash}`).
3. Once the threshold of partial signatures is met, **fetch the reconstructed full exit message** with `ExitController_getClusterExit[1]_v1` (`GET /v1/exp/exit/{lockHash}/{shareIdx}/{validatorPubkey}`) and broadcast it to the beacon chain.
