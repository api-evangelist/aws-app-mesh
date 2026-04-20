# AWS App Mesh (aws-app-mesh)
AWS App Mesh is a service mesh based on the Envoy proxy that provides application-level networking to make it easy for services to communicate with each other across multiple types of compute infrastructure including Amazon ECS, EKS, EC2, and Fargate. App Mesh standardizes service communication, giving end-to-end visibility and helping ensure high availability. Note: AWS App Mesh is deprecated; Amazon ECS Service Connect is the recommended replacement for new workloads.

**URL:** [https://aws.amazon.com/app-mesh/](https://aws.amazon.com/app-mesh/)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - AWS, Deprecated, Envoy, Microservices, Networking, Service Mesh

## Timestamps

- **Created:** 2026-03-16
- **Modified:** 2026-04-19

## APIs

### AWS App Mesh API
API for creating and managing App Mesh service meshes, virtual services, virtual nodes, virtual routers, routes, and gateway routes. The service is based on Envoy proxy and provides service discovery, traffic routing, and observability for microservices.

**Human URL:** [https://aws.amazon.com/app-mesh/](https://aws.amazon.com/app-mesh/)

#### Tags:

 - Deprecated, Envoy, Microservices, Networking, Service Mesh

#### Properties

- [Documentation](https://docs.aws.amazon.com/app-mesh/latest/APIReference/Welcome.html)
- [OpenAPI](openapi/aws-app-mesh-openapi.yaml)
- [APIReference](https://docs.aws.amazon.com/app-mesh/latest/APIReference/Welcome.html)
- [Authentication](https://docs.aws.amazon.com/app-mesh/latest/userguide/security-iam.html)
- [Quickstart](https://docs.aws.amazon.com/app-mesh/latest/userguide/getting-started-ecs.html)
- [Migration Guide to ECS Service Connect](https://aws.amazon.com/blogs/containers/migrating-from-aws-app-mesh-to-amazon-ecs-service-connect/)

## Common Properties

- [Website](https://aws.amazon.com/app-mesh/)
- [Documentation](https://docs.aws.amazon.com/app-mesh/)
- [GettingStarted](https://docs.aws.amazon.com/app-mesh/latest/userguide/getting_started.html)
- [Pricing](https://aws.amazon.com/app-mesh/pricing/)
- [FAQ](https://aws.amazon.com/app-mesh/faqs/)
- [Console](https://console.aws.amazon.com/appmesh/)
- [Support](https://aws.amazon.com/premiumsupport/)
- [StatusPage](https://health.aws.amazon.com/health/status)
- [TermsOfService](https://aws.amazon.com/service-terms/)
- [PrivacyPolicy](https://aws.amazon.com/privacy/)

## Features

| Name | Description |
|------|-------------|
| Service Mesh Management | Create and manage service meshes spanning Amazon ECS, EKS, EC2, and Fargate compute environments. |
| Virtual Node Configuration | Define virtual nodes representing actual services with listener ports, health checks, and service discovery backends. |
| Traffic Routing | Configure virtual routers and routes for weighted routing, retry policies, and timeout configurations. |
| Envoy Proxy Integration | Automatically injects and manages Envoy sidecar proxies for transparent service-to-service communication. |
| Observability | Export metrics, logs, and traces from Envoy proxies to AWS CloudWatch, X-Ray, and third-party tools. |
| mTLS Encryption | Enable mutual TLS encryption between services within the mesh for zero-trust networking. |
| Virtual Gateways | Configure ingress traffic from outside the mesh to virtual services using gateway routes. |
| Multi-Account Mesh Sharing | Share service meshes across AWS accounts using AWS Resource Access Manager. |

## Use Cases

| Name | Description |
|------|-------------|
| Microservices Communication | Standardize and control service-to-service networking for containerized microservices applications. |
| Traffic Management | Implement canary deployments, A/B testing, and weighted routing without application code changes. |
| Observability and Debugging | Capture end-to-end metrics and traces to identify performance bottlenecks and service failures. |
| Zero-Trust Networking | Enforce mTLS encryption between services for internal network security compliance. |

## Integrations

| Name | Description |
|------|-------------|
| Amazon ECS | Automatically inject Envoy sidecars into ECS task definitions. |
| Amazon EKS | Integrate with Kubernetes pod networking using the App Mesh controller for Kubernetes. |
| AWS X-Ray | Export distributed traces from Envoy proxies to X-Ray for performance analysis. |
| Amazon CloudWatch | Send Envoy proxy metrics to CloudWatch for monitoring and alerting. |
| AWS Cloud Map | Use Cloud Map for service discovery within the mesh. |
| Amazon EC2 | Run Envoy sidecar proxies alongside EC2-hosted services. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [AWS App Mesh API](openapi/aws-app-mesh-openapi.yaml)

### JSON Schema

333 schema files covering Mesh, VirtualNode, VirtualService, VirtualRouter, Route, VirtualGateway, GatewayRoute, and supporting types.

### JSON Structure

333 JSON Structure files converted from JSON Schema using json-structure.org/meta/core/v0.

### JSON-LD

20+ JSON-LD context files mapping App Mesh resource types and properties to linked data semantics.

### Examples

333 example JSON files generated from JSON Schema definitions.

## Capabilities

Naftiko capabilities organized as shared per-API definitions composed into customer-facing workflows.

### Shared Per-API Definitions

- [AWS App Mesh](capabilities/shared/app-mesh.yaml) — 6 operations for service mesh lifecycle management

### Workflow Capabilities

| Workflow | APIs Combined | Tools | Persona |
|----------|--------------|-------|---------|
| [Service Mesh Workflow](capabilities/service-mesh-workflow.yaml) | App Mesh | 6 | Platform Engineer |

## Vocabulary

- [AWS App Mesh Vocabulary](vocabulary/aws-app-mesh-vocabulary.yaml) — Unified taxonomy mapping 7 resources, 5 actions, 1 workflow, and 1 persona across operational (OpenAPI) and capability (Naftiko) dimensions

## Rules

- [AWS App Mesh Spectral Rules](rules/aws-app-mesh-spectral-rules.yml) — 20 rules across 7 categories enforcing AWS App Mesh API conventions

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
