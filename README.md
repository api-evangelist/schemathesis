# Schemathesis

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
