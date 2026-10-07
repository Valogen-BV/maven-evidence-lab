# Expected-result model

Each fixture will have a machine-readable expected-result document. The exact schema will be finalised during the project.

## Planned fields

- fixture identifier and version;
- input artefact paths and SHA-256 hashes;
- Maven coordinates and Package URL where determinable;
- directly observed metadata with its source location;
- Maven-resolved metadata with the resolution rule used;
- dependency relationships and scope;
- declared licence statements and detected licence-text observations;
- deliberately conflicting or unresolved facts;
- assertions applicable to each adapter boundary;
- assertions explicitly unsupported by an adapter;
- exact tool name, version, configuration and raw-output location;
- expected-result schema version and dataset licence.

## Result states

- `observed`: directly present in a bounded input.
- `resolved`: deterministically derived through documented Maven semantics.
- `conflicting`: two or more relevant sources disagree.
- `unknown`: the fixture intentionally contains insufficient information.
- `not_applicable`: outside the adapter's documented inspection boundary.

The model will not use an unqualified confidence score to turn ambiguity into certainty.

