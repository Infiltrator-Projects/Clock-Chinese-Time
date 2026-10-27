# Chinese-Time clock — model

**Stable ID:** `chinese-time` · **Kind:** `clock`

## Defined behaviour

Exact traditional double-hour partition of local civil time; no geographic solar event required.

**Historical interpretation:** Twelve Earthly Branch double-hours.

**Fidelity boundary:** Uses offset-based modern local time, not a pre-standardisation historic longitude observation.

This resource owns its clock rendering and next visible update boundary. The clock's display mode must not be confused with Common's elapsed-duration projection. Required location inputs must be validated, and unsupported solar events must not be fabricated. Model accuracy must not be overstated beyond this documented interpretation.

## Implementation status

The source, tests and combined package still belong to [Libraries/Common](https://github.com/Infiltrator-Projects/Libraries/tree/main/resources/temporal). This repository documents the independent `.so` resource that is intended to be migrated; it does **not** claim a working standalone installer or release.

## Source documentation

[Calendar's clock model matrix](https://github.com/Infiltrator-Projects/Calendar/blob/main/docs/MODELS.md) · [Historical fidelity audit](https://github.com/Infiltrator-Projects/Libraries/blob/main/docs/TEMPORAL_HISTORICAL_FIDELITY.md) · [Runtime ABI](https://github.com/Infiltrator-Projects/Libraries/blob/main/docs/TEMPORAL_PROVIDERS.md)

## Source copy status

The model-specific implementation and required helpers are now copied into this repository. Its behaviour was compared with the original Common 1.19.78 provider; this adds copy-regression evidence, not a new independent historical audit. See [source provenance](../SOURCE.md) and [validation results](../VALIDATION-RESULTS.json). The original Common implementation remains in place.
