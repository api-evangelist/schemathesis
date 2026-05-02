# Schemathesis

Schemathesis is a property-based API testing tool that automatically generates test cases from OpenAPI and GraphQL schemas to find bugs and specification violations. It uses the Hypothesis property-based testing framework to generate diverse, edge-case-covering test inputs from schema constraints, detecting server crashes, response schema violations, validation bypasses, and stateful bugs in multi-step workflows.

Used by Netflix, SAP, Red Hat, IBM, and JetBrains.

**Human URL:** [https://schemathesis.io](https://schemathesis.io)

## Resources

- [Documentation](https://schemathesis.readthedocs.io)
- [Getting Started](https://schemathesis.readthedocs.io/en/stable/getting-started.html)
- [GitHub Repository](https://github.com/schemathesis/schemathesis)
- [PyPI Package](https://pypi.org/project/schemathesis/)
- [Docker Image](https://hub.docker.com/r/schemathesis/schemathesis)
- [GitHub Action](https://github.com/schemathesis/action)
- [Changelog](https://github.com/schemathesis/schemathesis/releases)
- [Blog](https://schemathesis.io/blog)
- [Research Paper (ACM)](https://dl.acm.org/doi/10.1145/3510003.3510097)

## Features

- **Property-Based Testing** — Generates thousands of test cases automatically from schema type constraints, format rules, enums, and patterns
- **Schema-Driven Fuzzing** — Inputs are constrained by schema definitions for targeted, meaningful fuzzing
- **Response Validation** — Checks status codes, response bodies, content types, and headers against OpenAPI declarations
- **Stateful Testing** — Follows OpenAPI Links to generate multi-step workflow tests
- **Automatic Shrinking** — Minimizes failing cases to smallest reproducible curl command
- **CI/CD Native** — GitHub Actions (`schemathesis/action@v2`), GitLab CI, pytest integration

## Supported Specifications

- OpenAPI 2.0 (Swagger), 3.0.x, 3.1.x
- GraphQL schemas (SDL and introspection)

## Installation

```bash
pip install schemathesis
# or
uvx schemathesis run schema.json --url https://api.example.com
```

## Artifacts

### JSON Schema

- [schemathesis-config-schema.json](json-schema/schemathesis-config-schema.json) — JSON Schema for Schemathesis configuration

### JSON Structure

- [schemathesis-config-structure.json](json-structure/schemathesis-config-structure.json) — Document structure for .schemathesis.yml

### JSON-LD

- [schemathesis-context.jsonld](json-ld/schemathesis-context.jsonld) — Linked data context for Schemathesis vocabulary

### Examples

- [schemathesis-cli-test-example.json](examples/schemathesis-cli-test-example.json) — CLI test run with output example

### Vocabulary

- [schemathesis-vocabulary.yml](vocabulary/schemathesis-vocabulary.yml) — Domain vocabulary for Schemathesis concepts

## Maintainers

**Kin Lane** — kin@apievangelist.com
