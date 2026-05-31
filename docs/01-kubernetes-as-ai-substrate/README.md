# Act One: Kubernetes is the right place to run agentic AI

## 1) Introduction: the problem this session solves

- Agentic AI workloads do not behave like normal services.
- They are stateful, bursty, multi-step, and often span more infrastructure than a single cluster.
- This session focuses on what it takes to run AI at scale and keep it operable.

## 2) Why Kubernetes is the substrate for AI, and why self-manage

- This is not just "can Kubernetes handle AI?" but why teams build on Kubernetes instead of only consuming a fully managed AI stack.
- Owning the substrate provides:
  - Granularity of control over AI footprint
  - Data sovereignty
  - Cost control
  - Demonstrable value proof
  - Open tooling ecosystem (Karpenter, KEDA, DRA, Ray, KAITO)
- Address the AI iron triangle: quality, speed, and cost.
- Practitioner profile:
  - Teams running AI at a scale, cost, or sensitivity where managed-only options are not enough
  - Teams that want to compose their own platform rather than rent one
  - ISVs and cloud-agnostic teams operating across clouds and hybrid
- Kubernetes primitives that matter:
  - Declarative resource management
  - Scheduling across heterogeneous hardware
  - Namespace isolation for multi-tenant AI
  - Ecosystem support for operational complexity

## 3) How agentic workloads differ from traditional services

Three distinct workload types and operational profiles:

- Training: long-running, GPU-dense, checkpoint-dependent
- Inference: latency-sensitive, bursty, model-loading overhead
- Agentic orchestration: multi-step coordination and tool-call execution

Common friction points with default Kubernetes setups:

- Distributed execution coordination
- Heterogeneous hardware scheduling
- Scale-to-zero for inference
- Multi-node job coordination
