---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aembit-cloud-openapi-original.yml
  format: yaml
  label: Aembit Cloud API
  slug: aembit-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aembit/refs/heads/main/openapi/_original/aembit-cloud-openapi-original.yml
- filename: aembit-edge-openapi-original.yml
  format: yaml
  label: Aembit Edge API
  slug: aembit-edge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aembit/refs/heads/main/openapi/_original/aembit-edge-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Aembit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aembit secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Aembit
provider_slug: aembit
scheme_count: 2
schemes:
- api: Aembit Cloud API
  bearerFormat: Reference
  credential: Aembit API Token
  description: Authorization header using the Bearer scheme.
  issued_by: Aembit Admin UI, Profile screen
  lifetime: Not published.
  name: bearerAuth
  rotation: Not published; no token-rotation or revocation endpoint appears in the contract.
  scheme: bearer
  sources:
  - openapi/aembit-cloud-api-openapi.yml
  token_shape: Opaque reference token — bearerFormat is declared as "Reference", not JWT, so a client must not attempt to parse or introspect it.
  top_level_security: 'The Cloud API declares `security: [{}]` at the document root — an EMPTY requirement object, which in OpenAPI means security is OPTIONAL for every operation that does not override it. No operation overrides it. Read literally the contract states that all 165 operations may be called anonymously, which contradicts the documented bearer requirement and the 401 "Not Authenticated" response declared on 161 of them. Treated here as a contract defect, not as a real anonymous surface.'
  type: http
- additional_trust_providers_documented:
  - AWS ALB JWT (added 2026-08-05)
  - GCP IAP JWT (added 2026-08-19)
  - Azure managed identity
  - SPIFFE
  - Kerberos
  api: Aembit Edge API
  applies_to: POST /edge/v1/credentials (edge-api-get-credentials)
  bearerFormat: JWT
  bootstrap: 'The auth operation itself is unauthenticated by design. A Client Workload presents attestation evidence in an AuthRequest body and Aembit verifies it against a configured Trust Provider. This is the secretless bootstrap: the workload holds no credential before the call.'
  credential: Short-lived Edge access token
  description: Use Aembit Edge API access token obtained via the /edge/v1/auth endpoint.
  issued_by: POST /edge/v1/auth (operationId edge-api-auth)
  name: EdgeApiAuth
  scheme: bearer
  sources:
  - openapi/aembit-edge-api-openapi.yml
  supported_trust_providers:
  - AWS Metadata Service
  - AWS Role
  - GCP Identity Token
  - GitHub Action ID Token
  - GitLab Job ID Token
  - Kubernetes Service Account
  - OIDC ID Token
  - Terraform Cloud Identity Token
  token_shape: OAuth2-style TokenDTO carrying the access token and expiry details.
  top_level_security: 'security: [{EdgeApiAuth: []}] — correctly declared and applied.'
  trust_provider_note: The eight in supported_trust_providers are the set the Edge API's own operation description enumerates. The additional list is documented elsewhere in the platform docs and in the changelog; recorded separately so the contract's own statement stays distinguishable from the wider product surface.
  type: http
slug: aembit-authentication
source_filename: aembit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: searched\nsource: openapi/aembit-cloud-api-openapi.yml, openapi/aembit-edge-api-openapi.yml\ndocs: https://docs.aembit.io/dev-guide/api/\nnote: >-\n  Upgraded from the mechanical derivation, which deduplicated the two schemes into one because\n  both are http/bearer. They are NOT the same credential and must not be interchanged: the Cloud\n  API takes a long-lived opaque token a human generates in the console, and the Edge API takes a\n  short-lived JWT a workload earns by proving its identity. That distinction is the entire\n  product.\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: []\n  oauth2_flows: []\n  mutual_tls: false\n  openid_connect: false\n  scopes_published: false\n  scopes_note: >-\n    No OAuth 2.0 scopes exist on either API, so no scopes/ artifact is emitted. Authorization is\n    enforced by RBAC Roles plus the Resource Set boundary, not by token scopes.\nschemes:\n- name: bearerAuth\n  api: Aembit Cloud\
  \ API\n  type: http\n  scheme: bearer\n  bearerFormat: Reference\n  description: Authorization header using the Bearer scheme.\n  sources: [openapi/aembit-cloud-api-openapi.yml]\n  credential: Aembit API Token\n  issued_by: Aembit Admin UI, Profile screen\n  token_shape: >-\n    Opaque reference token — bearerFormat is declared as \"Reference\", not JWT, so a client must\n    not attempt to parse or introspect it.\n  lifetime: Not published.\n  rotation: Not published; no token-rotation or revocation endpoint appears in the contract.\n  top_level_security: >-\n    The Cloud API declares `security: [{}]` at the document root — an EMPTY requirement object,\n    which in OpenAPI means security is OPTIONAL for every operation that does not override it.\n    No operation overrides it. Read literally the contract states that all 165 operations may be\n    called anonymously, which contradicts the documented bearer requirement and the 401 \"Not\n    Authenticated\" response declared on 161 of\
  \ them. Treated here as a contract defect, not as a\n    real anonymous surface.\n- name: EdgeApiAuth\n  api: Aembit Edge API\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Use Aembit Edge API access token obtained via the /edge/v1/auth endpoint.\n  sources: [openapi/aembit-edge-api-openapi.yml]\n  credential: Short-lived Edge access token\n  issued_by: 'POST /edge/v1/auth (operationId edge-api-auth)'\n  token_shape: OAuth2-style TokenDTO carrying the access token and expiry details.\n  applies_to: 'POST /edge/v1/credentials (edge-api-get-credentials)'\n  top_level_security: 'security: [{EdgeApiAuth: []}] — correctly declared and applied.'\n  bootstrap: >-\n    The auth operation itself is unauthenticated by design. A Client Workload presents attestation\n    evidence in an AuthRequest body and Aembit verifies it against a configured Trust Provider.\n    This is the secretless bootstrap: the workload holds no credential before the call.\n  supported_trust_providers:\n\
  \  - AWS Metadata Service\n  - AWS Role\n  - GCP Identity Token\n  - GitHub Action ID Token\n  - GitLab Job ID Token\n  - Kubernetes Service Account\n  - OIDC ID Token\n  - Terraform Cloud Identity Token\n  additional_trust_providers_documented:\n  - AWS ALB JWT (added 2026-08-05)\n  - GCP IAP JWT (added 2026-08-19)\n  - Azure managed identity\n  - SPIFFE\n  - Kerberos\n  trust_provider_note: >-\n    The eight in supported_trust_providers are the set the Edge API's own operation description\n    enumerates. The additional list is documented elsewhere in the platform docs and in the\n    changelog; recorded separately so the contract's own statement stays distinguishable from\n    the wider product surface.\nauthorization:\n  model: RBAC + Resource Sets\n  roles_api: /api/v1/roles\n  resource_set_header: X-Aembit-ResourceSet\n  resource_set_type: uuid\n  note: >-\n    Authorization is two-dimensional: a Role grants permissions to an administrative user, and a\n    Resource Set partitions\
  \ which entities a request may touch. The Resource Set is carried as an\n    optional request header on effectively every operation and on the MCP Server; omitting it\n    falls back to the default Resource Set. An automated client should always set it explicitly.\n  sso:\n    api: /api/v1/sso-idps\n    signon_policies: [/api/v1/signin-policies, /api/v1/signin-policies/mfa, /api/v1/signin-policies/sso]\n    note: SAML/OIDC SSO and MFA sign-on policy are configurable for console users; they do not apply to API token auth.\nmcp_server_auth:\n  scheme: bearer\n  header: 'Authorization: Bearer <apiToken>'\n  credential: Same Aembit API Token as the Cloud API.\n  scoping: X-Aembit-ResourceSet (optional uuid)\n  cross_link: mcp/aembit-mcp.yml\ngaps:\n- 'security: [{}] at the Cloud API root makes authentication read as optional for all 165 operations.'\n- No published API token lifetime, rotation guidance, or revocation endpoint.\n- No OAuth 2.0 authorization-code or client-credentials flow for\
  \ third-party integrations against the Cloud API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aembit/refs/heads/main/authentication/aembit-authentication.yml
summary_line: http · 2 schemes
tags:
- Security
- Identity
- Access Management
- Workload Identity
- Non-Human Identity
- Secrets Management
- Zero Trust
- Agentic AI
- Model Context Protocol
- Authentication
- Authorization
- DevSecOps
- Cloud Security
---
