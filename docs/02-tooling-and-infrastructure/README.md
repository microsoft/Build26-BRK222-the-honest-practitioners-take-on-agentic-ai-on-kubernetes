# Act Two: Purpose-built tooling and managed infrastructure for AI at scale

## 4) Inference and serving: KAITO and AI Runway

- Start with practical production concerns: running models reliably.
- KAITO is used for simplified model serving on Kubernetes.
- AI Runway is positioned as an open-source inference platform to reduce the path from model validation to production deployment.
- Kubernetes-native capabilities highlighted:
  - Scaling configuration
  - Canary deployments
  - Rollback mechanisms
- This sets up a layer-cake progression:
  - Serve models reliably
  - Customize and train
  - Orchestrate agentic systems

## 5) Training and RL: Anyscale on Azure (managed Ray)

- There is a gap between default Kubernetes capabilities and production AI demands:
  - Distributed compute scheduling
  - Heterogeneous hardware coordination
  - Autoscaling for bursty inference
  - Multi-node job orchestration
- Ray is presented as the distributed compute framework that fills this gap.
- Anyscale on Azure provides an Azure-native experience on Azure Kubernetes Service.
- Practical outcomes highlighted:
  - Provision from Azure portal
  - Unified billing through Azure
  - Enterprise security via Microsoft Entra ID
  - Runtime in customer Azure Kubernetes Service environments

## 6) Agentic systems: skills, MCP, and Open Claw on Kubernetes

- With serving and training in place, next comes orchestration.
- Focus areas:
  - Building, registering, and calling skills/tools
  - MCP as connective tissue between agents, tools, and services
  - Where Kubernetes primitives (namespaces, RBAC, service mesh) help
- Open Claw is presented as part of agentic enablement.
- Why Kubernetes for the agent layer:
  - Session state handling
  - Multi-step coordination
  - Tool-call observability
  - Composable stack design

## 7) Azure Kubernetes Service substrate from single cluster to fleet

Announcements and capabilities highlighted:

- Azure Kubernetes Service Automatic with hosted system node pools
- Azure Container Linux
- Azure Kubernetes Service Bare Metal (public preview)
- Azure Kubernetes Fleet Manager for Arc-enabled clusters (GA)

Operational outcomes:

- Reduced system node management overhead
- Direct hardware access options for GPU performance-sensitive scenarios
- Progressive rollouts and policy consistency across cloud, on-premises, and edge
