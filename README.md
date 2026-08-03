# AWS App Mesh (aws-app-mesh)

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
