---
api_key_in:
- header
api_specs:
- filename: corestack-external-api-openapi-original.json
  format: json
  label: CoreStack External API
  slug: corestack-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/corestack/refs/heads/main/openapi/corestack-external-api-openapi-original.json
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Corestack Authentication
name_suffix: Authentication
oauth_flows: []
overview: CoreStack secures its APIs with apiKey and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CoreStack
provider_slug: corestack
scheme_count: 4
schemes:
- in: header
  name: auth_token
  note: The only securityDefinition declared in the published Swagger 2.0 document. The spec declares it but does NOT declare the companion X-Auth-User header, which the docs state is required on every call except the token operations — a real gap between the contract and the documentation.
  parameter: X-Auth-Token
  sources:
  - openapi/corestack-external-api-openapi-original.json
  surface: rest
  type: apiKey
- documented_only: true
  in: header
  name: auth_user
  note: Username of the tenant. Required on all operations except the AuthToken API. Not in the spec.
  parameter: X-Auth-User
  sources:
  - https://docs.corestack.io/docs/corestack-api-modules
  surface: rest
  type: apiKey
- authorizationUrl: https://cloud.corestack.io/mcp/oauth/authorize
  dynamic_client_registration: true
  flow: authorizationCode
  issuer: https://cloud.corestack.io/mcp
  name: mcp_oauth
  pkce: S256
  registrationUrl: https://cloud.corestack.io/mcp/oauth/register
  scopes:
  - openid
  - email
  - profile
  sources:
  - well-known/corestack-oauth-authorization-server.json
  - well-known/corestack-oauth-protected-resource.json
  surface: mcp
  tokenUrl: https://cloud.corestack.io/mcp/oauth/token
  type: oauth2
- companion_parameter: X-API-Secret-Key
  in: header
  name: mcp_api_keys
  parameter: X-API-Access-Key
  sources:
  - https://docs.corestack.io/docs/mcp-client-configuration
  surface: mcp
  type: apiKey
slug: corestack-authentication
source_filename: corestack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: searched\nsource: https://docs.corestack.io/docs/corestack-api-modules\ndocs:\n  rest: https://docs.corestack.io/docs/corestack-api-modules\n  auth_token_operation: https://docs.corestack.io/reference/authtoken\n  refresh_token_operation: https://docs.corestack.io/reference/refreshtoken\n  mcp: https://docs.corestack.io/docs/mcp-client-configuration\n  rbac: https://docs.corestack.io/docs/role-based-access-control-rbac\n  sso: https://docs.corestack.io/docs/setting-up-okta-sso\nspec_source: openapi/corestack-external-api-openapi-original.json\n\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  note: >-\n    Two distinct authentication systems, one per surface. The REST API uses a custom two-header\n    key-plus-token scheme with no OAuth anywhere in the 838-operation contract. The MCP server, added\n    later, uses either an OAuth 2.1 authorization-code + PKCE flow with RFC 7591 dynamic client\n    registration, or a\
  \ separate pair of API access/secret key headers. The two surfaces do not share\n    credentials or header names.\n\nschemes:\n- name: auth_token\n  surface: rest\n  type: apiKey\n  in: header\n  parameter: X-Auth-Token\n  sources:\n  - openapi/corestack-external-api-openapi-original.json\n  note: >-\n    The only securityDefinition declared in the published Swagger 2.0 document. The spec declares\n    it but does NOT declare the companion X-Auth-User header, which the docs state is required on\n    every call except the token operations — a real gap between the contract and the documentation.\n- name: auth_user\n  surface: rest\n  type: apiKey\n  in: header\n  parameter: X-Auth-User\n  sources:\n  - https://docs.corestack.io/docs/corestack-api-modules\n  documented_only: true\n  note: Username of the tenant. Required on all operations except the AuthToken API. Not in the spec.\n- name: mcp_oauth\n  surface: mcp\n  type: oauth2\n  flow: authorizationCode\n  pkce: S256\n  dynamic_client_registration:\
  \ true\n  issuer: https://cloud.corestack.io/mcp\n  authorizationUrl: https://cloud.corestack.io/mcp/oauth/authorize\n  tokenUrl: https://cloud.corestack.io/mcp/oauth/token\n  registrationUrl: https://cloud.corestack.io/mcp/oauth/register\n  scopes:\n  - openid\n  - email\n  - profile\n  sources:\n  - well-known/corestack-oauth-authorization-server.json\n  - well-known/corestack-oauth-protected-resource.json\n- name: mcp_api_keys\n  surface: mcp\n  type: apiKey\n  in: header\n  parameter: X-API-Access-Key\n  companion_parameter: X-API-Secret-Key\n  sources:\n  - https://docs.corestack.io/docs/mcp-client-configuration\n\ncredential_lifecycle:\n  long_lived:\n    name: Access Key + Secret Key\n    issued_by: Account Administrator, per user, via Identity and Access Management > Users\n    delivery: email\n    expiry: none stated — valid until manually revoked or regenerated\n    revocation: >-\n      Regenerating overwrites and immediately invalidates the previous pair. Keys stop working\
  \ when\n      the user is terminated or suspended; for SSO users, suspension in the org LDAP ends platform\n      access but the platform Access Key must be deleted separately.\n  short_lived:\n    name: Auth Token\n    minted_by: POST /v1/auth/tokens with {access_key, secret_key}\n    max_validity: 6 hours\n    documented_default: 1 hour, per the AuthToken reference page\n    refresh:\n      operation: POST /v1/auth/tokens/refresh\n      max_refreshes: 3\n      note: >-\n        Each refresh extends validity by another hour and increments refresh_count. After the third\n        refresh the token cannot be extended and a new AuthToken call is required.\n    expired_signal: 401 Unauthorized\n  note: >-\n    The docs carry two different validity numbers for the same token — \"valid only for an hour\" on\n    the AuthToken reference page and a \"maximum of 6 hours\" token-expiration policy table on the API\n    guide. Both are the provider's own published figures; recorded as-is rather than\
  \ reconciled.\n\nsso:\n  supported: true\n  documented_provider: Okta\n  operation: SsoRedirectUrl (POST /v1/sso_auth/tokens/{sso_name})\n  note: LDAP-backed identity; users are provisioned in CoreStack but authenticated by the org IdP.\n\nauthorization_model:\n  style: RBAC\n  scoping:\n  - master account\n  - tenant\n  - user group\n  - role\n  note: >-\n    Multi-tenant by design. Most operations require a tenant_id in the path, and many also require\n    an account ID; both are returned in the AuthToken response. Roles determine which modules and\n    APIs a user can reach. The MCP server explicitly inherits the caller's role — it grants nothing\n    additional.\n\ngaps:\n- The spec declares only X-Auth-Token; X-Auth-User is documented but absent from securityDefinitions.\n- No OAuth 2.0 on the REST surface at all, despite an enterprise, multi-tenant, RBAC-scoped API.\n- No scope model on REST — authorization is role-based and invisible to the contract.\n- Token validity is documented\
  \ inconsistently (1 hour vs 6 hours) across two provider pages.\n\nx-evidence:\n  fetched: '2026-08-11'\n  probes:\n  - url: https://api.corestack.io/v1/auth/tokens\n    method: POST\n    http_status: 400\n    body: '{\"message\": \"Please Provide Username/Password or AccessKey/SecretKey\"}'\n    note: Confirms the token endpoint is live and names the two accepted credential shapes.\n  - url: https://cloud.corestack.io/mcp\n    method: POST\n    http_status: 401\n    note: OAuth challenge naming the RFC 9728 resource metadata document.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corestack/refs/heads/main/authentication/corestack-authentication.yml
summary_line: apiKey/oauth2 · 4 schemes
tags:
- Cloud Governance
- FinOps
- Cloud Cost Management
- Cloud Security Posture Management
- Compliance
- Multi-Cloud
- CNAPP
- Policy as Code
- cloudops
- MCP
- agent-native
- Kubernetes
---
