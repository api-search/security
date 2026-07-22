---
api_key_in:
- header
auth_types:
- apiKey
- http
- oauth2
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Diagrid Authentication
name_suffix: Authentication
oauth_flows:
- browser-login
overview: Diagrid secures its APIs with apiKey, http, oauth2, and mutualTLS across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the browser-login flow(s).
provider_name: Diagrid
provider_slug: diagrid
scheme_count: 5
schemes:
- description: Scoped application API token presented on every Dapr API call to the regional Catalyst gateway; transport is TLS. Created/managed via `diagrid apikey` and service-account API keys.
  docs: https://docs.diagrid.io/references/catalyst/cli-reference/apikey/
  in: header
  name: AppApiToken
  type: apiKey
- description: Named machine tokens tied to a role assignment, with configurable expiry and optional project scope, for automation and CI.
  docs: https://docs.diagrid.io/references/catalyst/cli-reference/serviceaccount/
  in: header
  name: ServiceAccountToken
  type: apiKey
- description: Interactive browser-based login used by the diagrid CLI; access and identity tokens can be printed via `diagrid auth print-access-token` / `print-identity-token`.
  docs: https://docs.diagrid.io/references/catalyst/cli-reference/auth/
  flow: browser-login
  name: CliLogin
  type: oauth2
- description: SAML 2.0 SSO via enterprise identity providers (Catalyst Enterprise).
  name: SamlSso
  plans:
  - enterprise
  type: openIdConnect
- description: SPIFFE-based mutual TLS between in-platform workloads; each data-plane component receives a short-lived X.509 SVID signed by Dapr Sentry, rotated automatically.
  docs: https://docs.diagrid.io/concepts/security
  name: WorkloadMtls
  type: mutualTLS
slug: diagrid-authentication
source_filename: diagrid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.diagrid.io/concepts/security\ndocs: https://docs.diagrid.io/concepts/identities\nnotes: >-\n  Derived from Diagrid Catalyst security/identity docs (no public OpenAPI is\n  published; the platform exposes the Dapr HTTP/gRPC APIs behind a regional\n  gateway). Application calls present a scoped app API token over TLS; human and\n  automation access is role-based; internal workloads use SPIFFE X.509 SVID mTLS.\nsummary:\n  types: [apiKey, http, oauth2, mutualTLS]\n  api_key_in: [header]\n  oauth2_flows: [browser-login]\n  workload_identity: SPIFFE-X.509-SVID\nschemes:\n  - name: AppApiToken\n    type: apiKey\n    in: header\n    description: >-\n      Scoped application API token presented on every Dapr API call to the\n      regional Catalyst gateway; transport is TLS. Created/managed via\n      `diagrid apikey` and service-account API keys.\n    docs: https://docs.diagrid.io/references/catalyst/cli-reference/apikey/\n\
  \  - name: ServiceAccountToken\n    type: apiKey\n    in: header\n    description: >-\n      Named machine tokens tied to a role assignment, with configurable expiry\n      and optional project scope, for automation and CI.\n    docs: https://docs.diagrid.io/references/catalyst/cli-reference/serviceaccount/\n  - name: CliLogin\n    type: oauth2\n    flow: browser-login\n    description: >-\n      Interactive browser-based login used by the diagrid CLI; access and\n      identity tokens can be printed via `diagrid auth print-access-token` /\n      `print-identity-token`.\n    docs: https://docs.diagrid.io/references/catalyst/cli-reference/auth/\n  - name: SamlSso\n    type: openIdConnect\n    description: SAML 2.0 SSO via enterprise identity providers (Catalyst Enterprise).\n    plans: [enterprise]\n  - name: WorkloadMtls\n    type: mutualTLS\n    description: >-\n      SPIFFE-based mutual TLS between in-platform workloads; each data-plane\n      component receives a short-lived X.509 SVID\
  \ signed by Dapr Sentry, rotated\n      automatically.\n    docs: https://docs.diagrid.io/concepts/security\nroles:\n  - Admin\n  - Operator\n  - Consumer\n  - Viewer\naccess_policies:\n  description: >-\n    Runtime behavior is governed declaratively by access policies controlling\n    which applications can be invoked and which components they can access.\n  docs: https://docs.diagrid.io/concepts/policies\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/diagrid/refs/heads/main/authentication/diagrid-authentication.yml
summary_line: apiKey/http/oauth2/mutualTLS · 5 schemes
tags:
- Company
- Developer Tools
- AI Agents
- Durable Execution
- Workflows
- Dapr
- Model Context Protocol
- Microservices
- Cloud Native
- Distributed Systems
---
