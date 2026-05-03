# Volcano

Volcano is a CNCF incubating batch processing and high-performance computing (HPC) scheduler for Kubernetes. It extends Kubernetes with three CRDs — Job (vcjob), Queue, and PodGroup — providing gang scheduling, fair-share queue scheduling, and job lifecycle management for ML training, big data, and scientific computing workloads.

- **Website:** [https://volcano.sh/](https://volcano.sh/)
- **Documentation:** [https://volcano.sh/en/docs/](https://volcano.sh/en/docs/)
- **GitHub:** [https://github.com/volcano-sh/volcano](https://github.com/volcano-sh/volcano)
- **CNCF:** [https://www.cncf.io/projects/volcano/](https://www.cncf.io/projects/volcano/)

## APIs

### Volcano Job API (vcjob)

Kubernetes CRD for managing batch workloads with multiple task groups, lifecycle policies, gang scheduling, and framework plugins.

- **Documentation:** [https://volcano.sh/en/docs/vcjob/](https://volcano.sh/en/docs/vcjob/)
- **OpenAPI:** [openapi/volcano-job-openapi.yml](openapi/volcano-job-openapi.yml)
- **JSON Schema:** [json-schema/volcano-job-schema.json](json-schema/volcano-job-schema.json)

### Volcano Queue API

Kubernetes CRD for managing scheduling queues with weight-based fair sharing and resource quotas.

- **Documentation:** [https://volcano.sh/en/docs/v1-10-0/queue/](https://volcano.sh/en/docs/v1-10-0/queue/)
- **OpenAPI:** [openapi/volcano-queue-openapi.yml](openapi/volcano-queue-openapi.yml)

### Volcano PodGroup API

Kubernetes CRD for gang scheduling — defines a group of pods that must all be scheduled together.

- **Documentation:** [https://volcano.sh/en/docs/podgroup/](https://volcano.sh/en/docs/podgroup/)
- **OpenAPI:** [openapi/volcano-podgroup-openapi.yml](openapi/volcano-podgroup-openapi.yml)

## Artifacts

### OpenAPI Specifications

| Spec | Description |
|------|-------------|
| [openapi/volcano-job-openapi.yml](openapi/volcano-job-openapi.yml) | Volcano Job CRD API |
| [openapi/volcano-queue-openapi.yml](openapi/volcano-queue-openapi.yml) | Volcano Queue CRD API |
| [openapi/volcano-podgroup-openapi.yml](openapi/volcano-podgroup-openapi.yml) | Volcano PodGroup CRD API |

### JSON Schema

| Schema | Description |
|--------|-------------|
| [json-schema/volcano-job-schema.json](json-schema/volcano-job-schema.json) | Volcano Job resource schema |

### JSON Structure

| Structure | Description |
|-----------|-------------|
| [json-structure/volcano-job-structure.json](json-structure/volcano-job-structure.json) | Job field-level documentation |

### JSON-LD Context

| Context | Description |
|---------|-------------|
| [json-ld/volcano-context.jsonld](json-ld/volcano-context.jsonld) | Linked data context for Volcano resources |

### Spectral Rules

| Ruleset | Description |
|---------|-------------|
| [rules/volcano-rules.yml](rules/volcano-rules.yml) | Volcano API linting rules |

### Naftiko Capabilities

| Capability | Description |
|------------|-------------|
| [capabilities/batch-workload-management.yaml](capabilities/batch-workload-management.yaml) | Unified batch workload management (10 tools) |
| [capabilities/shared/volcano-jobs.yaml](capabilities/shared/volcano-jobs.yaml) | Shared Volcano Job API definition |
| [capabilities/shared/volcano-queues.yaml](capabilities/shared/volcano-queues.yaml) | Shared Volcano Queue API definition |
| [capabilities/shared/volcano-podgroups.yaml](capabilities/shared/volcano-podgroups.yaml) | Shared Volcano PodGroup API definition |

### Examples

| Example | Description |
|---------|-------------|
| [examples/volcano-createNamespacedJob-example.json](examples/volcano-createNamespacedJob-example.json) | Submit a PyTorch distributed training job |
| [examples/volcano-listQueues-example.json](examples/volcano-listQueues-example.json) | List scheduling queues |
| [examples/volcano-createNamespacedPodGroup-example.json](examples/volcano-createNamespacedPodGroup-example.json) | Create a PodGroup for Spark |

### Vocabulary

| Vocabulary | Description |
|------------|-------------|
| [vocabulary/volcano-vocabulary.yml](vocabulary/volcano-vocabulary.yml) | Volcano domain vocabulary |

## Scope

- **Type:** Index
- **Tags:** Batch Processing, Cloud Native, HPC, Kubernetes, Scheduling, Machine Learning, CNCF

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
