---
api_key_in: []
api_specs:
- filename: agentgateway-config-api-openapi.yml
  format: yaml
  label: AgentGateway Config API
  slug: agentgateway-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentgateway/refs/heads/main/openapi/agentgateway-config-api-openapi.yml
- filename: agentgateway-debug-api-openapi.yml
  format: yaml
  label: AgentGateway Debug API
  slug: agentgateway-debug-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentgateway/refs/heads/main/openapi/agentgateway-debug-api-openapi.yml
- filename: agentgateway-lifecycle-api-openapi.yml
  format: yaml
  label: AgentGateway Lifecycle API
  slug: agentgateway-lifecycle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentgateway/refs/heads/main/openapi/agentgateway-lifecycle-api-openapi.yml
- filename: agentgateway-logging-api-openapi.yml
  format: yaml
  label: AgentGateway Logging API
  slug: agentgateway-logging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentgateway/refs/heads/main/openapi/agentgateway-logging-api-openapi.yml
- filename: agentgateway-memory-api-openapi.yml
  format: yaml
  label: AgentGateway Memory API
  slug: agentgateway-memory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentgateway/refs/heads/main/openapi/agentgateway-memory-api-openapi.yml
- filename: agentgateway-profiling-api-openapi.yml
  format: yaml
  label: AgentGateway Profiling API
  slug: agentgateway-profiling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentgateway/refs/heads/main/openapi/agentgateway-profiling-api-openapi.yml
auth_types: []
description: Authentication for agentgateway has two distinct sides and they must not be conflated. (1) The ADMIN/DEBUG API this repo describes in openapi/ has NO authentication at all - it is protected by binding to loopback. (2) The gateway's DATA PLANE offers a rich inbound and backend authentication toolkit that YOU configure for the traffic passing through. Nothing here is a credential you obtain from agentgateway; there is no account, no key issuance, no signup.
kind: authentication
layout: security
method: searched
name: Agentgateway Authentication
name_suffix: Authentication
oauth_flows: []
overview: AgentGateway declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: AgentGateway
provider_slug: agentgateway
scheme_count: 0
schemes: []
slug: agentgateway-authentication
source_filename: agentgateway-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: searched\nsource: https://agentgateway.dev/docs/standalone/latest/configuration/security/ (jwt-authn, apikey-authn, basic-authn, oidc, mcp-authn, mcp-authz, external-authz, backend-authn/*) + https://agentgateway.dev/docs/standalone/latest/operations/debug/\nprovider: AgentGateway\nproviderId: agentgateway\ndescription: >-\n  Authentication for agentgateway has two distinct sides and they must not be conflated. (1) The\n  ADMIN/DEBUG API this repo describes in openapi/ has NO authentication at all - it is protected by\n  binding to loopback. (2) The gateway's DATA PLANE offers a rich inbound and backend authentication\n  toolkit that YOU configure for the traffic passing through. Nothing here is a credential you obtain\n  from agentgateway; there is no account, no key issuance, no signup.\nadmin_api:\n  schemes: []\n  authentication: none\n  transport_protection: loopback-bind\n  default_bind: 127.0.0.1:15000\n  configurable_via: adminAddr\n\
  \  applies_to:\n    - openapi/agentgateway-config-api-openapi.yml\n    - openapi/agentgateway-debug-api-openapi.yml\n    - openapi/agentgateway-lifecycle-api-openapi.yml\n    - openapi/agentgateway-logging-api-openapi.yml\n    - openapi/agentgateway-memory-api-openapi.yml\n    - openapi/agentgateway-profiling-api-openapi.yml\n  source: https://agentgateway.dev/docs/standalone/latest/operations/debug/\n  note: >-\n    Verbatim from the docs: \"The admin interface binds to the loopback interface, so only a client on\n    the same host can reach it. Keep it that way. Endpoints such as /quitquitquit and /config_dump shut\n    down the proxy and dump its full configuration to any caller that can open a connection.\" The\n    security model is network placement, not a credential. A derived securityScheme block would be a\n    fabrication - derive-authentication.py correctly produced zero profiles for this repo.\ndata_plane_inbound:\n  description: Authentication policies agentgateway can enforce\
  \ on traffic arriving at a listener or route.\n  methods:\n    - id: jwt\n      name: JWT authentication\n      type: http-bearer\n      attaches_to: [listener, route]\n      docs: https://agentgateway.dev/docs/standalone/latest/configuration/security/jwt-authn/\n      detail: >-\n        Validates a bearer JWT against a JWKS URL. Fields: issuer, audiences, jwks, requiredClaims\n        (default [\"exp\"]). Since 1.5.0 the `iss` claim is REQUIRED when `issuer` is set, and `aud` is\n        REQUIRED when `audiences` is a non-empty list - a behaviour change that rejects tokens that\n        previously passed. Verified claims are exposed to later policies as the CEL `jwt.*` context.\n    - id: apikey\n      name: API key authentication\n      type: apiKey\n      attaches_to: [listener, route]\n      docs: https://agentgateway.dev/docs/standalone/latest/configuration/security/apikey-authn/\n      detail: >-\n        Keys carry metadata that later policies can read via the CEL `apiKey` context\
  \ (for example to\n        set an x-authenticated-user header). Keys created in the admin UI or through the admin API\n        carry agentgateway-managed metadata under the reserved `agentgateway.dev/` prefix - since\n        1.5.0 the identifier moved from metadata.id to metadata[\"agentgateway.dev/id\"], a new\n        metadata[\"agentgateway.dev/createdAt\"] was added, and user-supplied fields using that prefix\n        are rejected. API keys also carry LLM budgets and per-key model access lists.\n    - id: basic\n      name: Basic authentication\n      type: http-basic\n      attaches_to: [listener, route]\n      docs: https://agentgateway.dev/docs/standalone/latest/configuration/security/basic-authn/\n    - id: oidc\n      name: OIDC browser authentication\n      type: openIdConnect\n      attaches_to: [route]\n      docs: https://agentgateway.dev/docs/standalone/latest/configuration/security/oidc/\n      detail: Interactive browser login, also the documented way to put a login in\
  \ front of the agentgateway UI.\n    - id: mcp-authn\n      name: MCP authentication\n      type: oauth2\n      attaches_to: [route]\n      docs: https://agentgateway.dev/docs/standalone/latest/configuration/security/mcp-authn/\n      detail: >-\n        Applies the MCP authorization spec in front of a fronted MCP server. Returns 401 Unauthorized\n        with a WWW-Authenticate header to unauthenticated callers, and SERVES the discovery documents\n        the client then fetches - /.well-known/oauth-protected-resource/{path} (RFC 9728) and\n        /.well-known/oauth-authorization-server/{path} (RFC 8414), plus a proxied dynamic client\n        registration endpoint (RFC 7591) where the identity provider needs one. Modes: `strict`\n        (default, a valid token from a configured issuer is required) and permissive variants.\n        Provider adapters exist for auth0, authentik, descope, keycloak and okta; Okta requires an\n        explicit `jwks` because it publishes keys at {issuer}/v1/keys.\n\
  \    - id: mcp-authz\n      name: MCP authorization\n      type: policy\n      attaches_to: [route, backend]\n      docs: https://agentgateway.dev/docs/standalone/latest/configuration/security/mcp-authz/\n      detail: Per-tool authorization over MCP method calls, evaluated after authentication.\n    - id: external-authz\n      name: External authorization (ext_authz)\n      type: delegated\n      attaches_to: [listener, route, backend]\n      docs: https://agentgateway.dev/docs/standalone/latest/configuration/security/external-authz/\n      detail: Delegates the allow/deny decision to an external policy server.\n    - id: network-authz\n      name: Network authorization\n      type: l4-acl\n      attaches_to: [frontend]\n      docs: https://agentgateway.dev/docs/standalone/latest/configuration/security/network-authz/\n      detail: L4 transport-level access control, applied before HTTP policy.\ndata_plane_backend:\n  description: How agentgateway authenticates ITSELF to the upstreams\
  \ it proxies to.\n  methods:\n    - id: static-key\n      name: Static keys and passthrough\n      docs: https://agentgateway.dev/docs/standalone/latest/configuration/security/backend-authn/key/\n    - id: jwt-sign\n      name: Signed JWT assertion (jwtSign)\n      docs: https://agentgateway.dev/docs/standalone/latest/configuration/security/backend-authn/jwt-sign/\n      detail: For upstreams that refuse a durable credential, such as Snowflake.\n    - id: oauth-token-exchange\n      name: OAuth token exchange (RFC 8693)\n      docs: https://agentgateway.dev/docs/standalone/latest/configuration/security/backend-authn/oauth-token-exchange/\n    - id: cross-app-access\n      name: Cross App Access (ID-JAG)\n      docs: https://agentgateway.dev/docs/standalone/latest/configuration/security/backend-authn/cross-app-access/\n    - id: aws\n      name: AWS SigV4 request signing\n      docs: https://agentgateway.dev/docs/standalone/latest/configuration/security/backend-authn/providers/aws/\n  \
  \  - id: gcp\n      name: Google Cloud credentials\n      docs: https://agentgateway.dev/docs/standalone/latest/configuration/security/backend-authn/providers/gcp/\n    - id: azure\n      name: Microsoft Entra ID token\n      docs: https://agentgateway.dev/docs/standalone/latest/configuration/security/backend-authn/providers/azure/\n    - id: copilot\n      name: GitHub Copilot token\n      docs: https://agentgateway.dev/docs/standalone/latest/configuration/security/backend-authn/providers/copilot/\n    - id: backend-tls\n      name: Backend TLS\n      docs: https://agentgateway.dev/docs/standalone/latest/configuration/security/backend-tls/\n    - id: spiffe\n      name: SPIFFE workload identity mTLS\n      docs: https://github.com/agentgateway/agentgateway/tree/main/examples/traffic-spiffe\nscopes:\n  applicable: false\n  note: >-\n    Agentgateway issues no OAuth scopes of its own. Scopes belong to whichever identity provider a\n    deployment configures; agentgateway validates the resulting\
  \ token. No scopes/ artifact is written -\n    an empty scope registry would misrepresent the product.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentgateway/refs/heads/main/authentication/agentgateway-authentication.yml
summary_line: 0 schemes
tags:
- AI Gateway
- API Gateway
- MCP
- LLM
- Agent-to-Agent
- Open-Source
- CNCF
- Observability
- Security
---
