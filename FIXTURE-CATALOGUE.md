# Proposed fixture catalogue

The funded scope targets at least 20 synthetic fixture families. Some families may contain several variants.

1. Direct dependency with complete coordinates and licence.
2. Version inherited from a parent POM.
3. Licence inherited from a parent POM.
4. Version supplied by an imported BOM.
5. Version supplied through a Maven property.
6. Nested property indirection.
7. Active-by-default Maven profile.
8. Multi-module reactor with inter-module dependency.
9. Aggregator POM versus parent POM distinction.
10. Dependency relocation.
11. Classifier-specific artefact.
12. Optional dependency.
13. Provided and system-scoped dependencies.
14. Shaded JAR with original dependency metadata.
15. Shaded JAR with incomplete metadata.
16. Nested JAR.
17. Vendored third-party JAR outside normal dependency resolution.
18. JAR with embedded `pom.properties` but no embedded POM.
19. Conflicting POM, manifest and `pom.properties` versions.
20. Licence declared in POM but absent from the JAR.
21. Licence file present in the JAR but absent from the POM.
22. Multiple licence declarations and SPDX expression mapping.
23. Snapshot-style version and timestamped artefact distinction.
24. Invalid or absent Package URL candidate.
25. Checksum mismatch represented as an intentionally unresolved case.

## Fixture rules

- Use synthetic names and minimal code.
- Build deterministically where Maven permits it.
- Record exact inputs, hashes and expected observations.
- Avoid dependencies that require redistribution of restricted content.
- Do not execute the produced artefacts during inspection.

