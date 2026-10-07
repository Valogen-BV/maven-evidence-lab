# Maven Evidence Lab

Maven Evidence Lab is a proposed open conformance corpus and Java test harness for package metadata in difficult Java/Maven/JAR scenarios.

## Problem

Maven metadata can come from a source POM, an effective POM, an imported BOM, an embedded `META-INF/maven/.../pom.properties`, a JAR manifest, licence files or repository metadata. These sources can be incomplete or contradictory. SBOM generators and package scanners also inspect different boundaries, which makes differences hard to reproduce and discuss.

The project will provide small synthetic fixtures with explicit expected observations. Tool adapters will run compatible open-source tools against the same inputs and preserve their raw outputs. The aim is reproducible testing and better upstream issue reports; not a new scanner, a universal ranking or a legal/security certification.

## Planned first release

- Java 17 command-line harness built with Maven Wrapper, JUnit 5 and Jackson.
- At least 20 synthetic Maven/JAR fixture families.
- Machine-readable expected-result data.
- Adapters for at least three compatible open-source tools.
- JSON and concise human-readable reports.
- CI examples and contributor documentation.

See [the fixture catalogue](docs/FIXTURE-CATALOGUE.md), [expected-result model](docs/EXPECTED-RESULTS.md) and [roadmap](ROADMAP.md).

## Boundaries

- Java/Maven/JAR only in the first release.
- No vulnerability database or vulnerability scanner.
- No execution of inspected fixture artefacts.
- No customer or proprietary code in the corpus.
- No generative AI functionality.
- Results describe tool observations within a documented boundary; they do not certify legal compliance or security.

## Intended licences

- Harness, executable fixture projects and documentation: Apache License 2.0.
- Original machine-readable expected-result datasets: CC0 1.0.

Full licence texts and per-file SPDX identifiers will be added before the first public release.

## Status

Funding-application preparation. No implementation has started and no grant-funded work is being claimed before project selection.

