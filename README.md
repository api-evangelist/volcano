# Volcano (volcano)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Volcano is a CNCF incubating batch processing and high-performance computing (HPC) scheduler for Kubernetes. It provides advanced scheduling capabilities including gang scheduling, fair-share scheduling, queue management, and job lifecycle management for batch workloads such as machine learning training, big data processing, and scientific computing. Volcano extends Kubernetes with three CRDs: Job (vcjob), Queue, and PodGroup.

**APIs.json:** [https://volcano.sh](https://volcano.sh)

## Scope

- **Type:** Index

## Tags

- Batch Processing
- Cloud Native
- HPC
- Incubating
- Kubernetes
- Scheduling
- Machine Learning

## Timestamps

- **Created:** 2026-03-16
- **Modified:** 2026-05-19

## APIs

### Volcano Batch Scheduling API

Volcano extends Kubernetes with CRDs for batch workload management. The Job resource defines batch workloads with multiple task types and lifecycle policies. Queue resources manage job scheduling with weight-based fair sharing and resource quotas. Volcano supports gang scheduling ensuring all pods in a group are scheduled together, and integrates with frameworks like TensorFlow, PyTorch, Spark, and MPI.

- **Human URL:** [https://volcano.sh/en/docs/](https://volcano.sh/en/docs/)

#### Tags

- Batch Scheduling
- Gang Scheduling
- Queues

#### Properties

- [Documentation](https://volcano.sh/en/docs/)
- [Reference](https://volcano.sh/en/docs/vcjob/)
- [Getting Started](https://volcano.sh/en/docs/installation/)
- [OpenAPI](openapi/volcano-job-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/volcano-job.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/volcano-job.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/volcano-job-schema.json) — [JSON Schema](https://json-schema.org/specification)

### Volcano Queue API

Kubernetes CRD for defining and managing job queues in Volcano. Queues collect PodGroups and support weight-based fair-share scheduling and resource quotas, providing the primary mechanism for multi-tenant resource partitioning and priority-based job admission.

- **Human URL:** [https://volcano.sh/en/docs/v1-10-0/queue/](https://volcano.sh/en/docs/v1-10-0/queue/)

#### Tags

- Batch Scheduling
- Kubernetes
- Multi-Tenancy
- Queues
- Resource Management

#### Properties

- [Documentation](https://volcano.sh/en/docs/v1-10-0/queue/)
- [OpenAPI](openapi/volcano-queue-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/volcano-queue.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/volcano-queue.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Volcano PodGroup API

Kubernetes CRD that represents a group of pods with strong association, used as the unit of gang scheduling in Volcano. PodGroups define the minimum number of pods that must be scheduled together, enabling all-or-nothing scheduling semantics for distributed training and computing workloads.

- **Human URL:** [https://volcano.sh/en/docs/podgroup/](https://volcano.sh/en/docs/podgroup/)

#### Tags

- Batch Scheduling
- Distributed Computing
- Gang Scheduling
- Kubernetes
- Pod Management

#### Properties

- [Documentation](https://volcano.sh/en/docs/podgroup/)
- [OpenAPI](openapi/volcano-podgroup-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/volcano-podgroup.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/volcano-podgroup.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/philips-volcano)
- [Website](https://volcano.sh/en/)
- [JSON-LD](json-ld/volcano-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [JSON Schema](json-schema/volcano-job-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/volcano-job-structure.json)
- [Vocabulary](vocabulary/volcano-vocabulary.yml)
- [Spectral Rules](rules/volcano-rules.yml)
- [Documentation](https://volcano.sh/en/docs/)
- [Getting Started](https://volcano.sh/en/docs/installation/)
- [Blog](https://volcano.sh/en/blog/)
- [GitHub Organization](https://github.com/volcano-sh)
- [GitHub Repository](https://github.com/volcano-sh/volcano)
- [Community](https://github.com/volcano-sh/community)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
