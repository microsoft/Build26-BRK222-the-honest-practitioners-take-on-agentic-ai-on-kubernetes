# Act Three: What this looks like in practice

Estimated time: 10 minutes

## 8) Customer architectures in practice

Short architecture vignettes aligned to the layer-cake model (serving -> training/RL -> agentic -> platform substrate):

- Vignette 1: Serving and inference at scale
  - Open-source models on Azure Kubernetes Service with KAITO and AI Runway
  - Architecture shape: model registry -> KAITO workspace -> autoscaled inference pools on GPU node pools
  - Burst handling with KEDA and Karpenter
- Vignette 2: Training/RL on Azure Kubernetes Service
  - Distributed training pattern with Ray/Anyscale
  - Multi-node GPU coordination and checkpointing focus
- Vignette 3: Agentic system in production
  - MCP-based agent layer on Azure Kubernetes Service
  - Agents calling tools/skills with session state in-cluster
  - Fleet-managed deployment across regions

## 9) What is available and what to do next

Practitioner's checklist:

- Start with core Kubernetes primitives
- Build the agent layer with MCP, skills, and Open Claw
- Choose tooling by build-vs-buy posture
- For training/RL, evaluate Ray and Anyscale patterns
- For inference/serving, evaluate KAITO and AI Runway
- Invest in fleet-level operations early; AI workloads can outgrow one cluster quickly

## Suggested attendee follow-up

- Start with the labs and links in the repository resources section.
- Explore the related LAB510 content for hands-on implementation patterns.
- Use the technology links in the main README to go deeper on specific platform components.
