# Volcano (volcano)

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
