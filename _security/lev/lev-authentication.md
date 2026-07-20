---
api_key_in: []
api_specs:
- filename: lev-openapi-original.json
  format: json
  label: Lev API
  slug: lev-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lev/refs/heads/main/openapi/lev-openapi-original.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Lev Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Lev secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Lev
provider_slug: lev
scheme_count: 2
schemes:
- bearerFormat: API Key or JWT
  credential_kinds:
  - account_binding: API keys are bound to one account at creation time
    kind: api-key
    lifetime: long-lived
    management_operations:
    - postApiKeys
    - getApiKeys
    - deleteApiKeysKeyId
    prefix: lev_sk_
    use: server-to-server integrations
    validate_endpoint: POST /api/external/v2/auth/validate-api-key
    validate_operation: postAuthValidateApiKey
  - algorithm: RS256
    issuer: https://auth.lev.com/
    kind: jwt
    lifetime: short-lived
    multi_account: JWT users with membership on multiple accounts must send X-Active-Account with the account slug; this header does not apply to API keys.
    provider: Auth0
    use: interactive clients
  docs: https://www.lev.com/docs/build/authentication
  header: 'Authorization: Bearer <token>'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/lev-openapi-original.json
  type: http
- applies_to: hosted MCP server at https://mcp.lev.com/mcp
  docs: https://www.lev.com/docs/build/mcp/auth
  dynamic_client_registration: true
  flows:
  - authorizationUrl: https://auth.lev.com/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    pkce: true
    registrationUrl: https://auth.lev.com/oidc/register
    revocationUrl: https://auth.lev.com/oauth/revoke
    scopes:
    - openid
    - email
    - offline_access
    tokenUrl: https://auth.lev.com/oauth/token
  issuer: https://auth.lev.com/
  name: mcpOAuth
  protected_resource_metadata: well-known/lev-oauth-protected-resource.json
  source: well-known/lev-oauth-authorization-server.json
  type: oauth2
slug: lev-authentication
source_filename: lev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/lev-openapi-original.json\ndocs: https://www.lev.com/docs/build/authentication\nsummary:\n  types:\n  - http\n  - oauth2\n  http_schemes:\n  - bearer\n  oauth2_flows:\n  - authorizationCode\n  credential_kinds:\n  - api-key\n  - jwt\n  note: The OpenAPI declares a single `bearerAuth` HTTP bearer scheme whose bearerFormat\n    is \"API Key or JWT\". The docs expand this into two distinct credential kinds carried\n    on the same Authorization header, plus a separate OAuth 2.1 authorization-code\n    flow used by the hosted MCP server.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key or JWT\n  header: 'Authorization: Bearer <token>'\n  sources:\n  - openapi/lev-openapi-original.json\n  docs: https://www.lev.com/docs/build/authentication\n  credential_kinds:\n  - kind: api-key\n    prefix: lev_sk_\n    lifetime: long-lived\n    use: server-to-server integrations\n    account_binding:\
  \ API keys are bound to one account at creation time\n    validate_operation: postAuthValidateApiKey\n    validate_endpoint: POST /api/external/v2/auth/validate-api-key\n    management_operations:\n    - postApiKeys\n    - getApiKeys\n    - deleteApiKeysKeyId\n  - kind: jwt\n    issuer: https://auth.lev.com/\n    provider: Auth0\n    algorithm: RS256\n    lifetime: short-lived\n    use: interactive clients\n    multi_account: JWT users with membership on multiple accounts must send X-Active-Account\n      with the account slug; this header does not apply to API keys.\n- name: mcpOAuth\n  type: oauth2\n  source: well-known/lev-oauth-authorization-server.json\n  docs: https://www.lev.com/docs/build/mcp/auth\n  applies_to: hosted MCP server at https://mcp.lev.com/mcp\n  issuer: https://auth.lev.com/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.lev.com/authorize\n    tokenUrl: https://auth.lev.com/oauth/token\n    revocationUrl: https://auth.lev.com/oauth/revoke\n\
  \    registrationUrl: https://auth.lev.com/oidc/register\n    pkce: true\n    code_challenge_methods:\n    - S256\n    scopes:\n    - openid\n    - email\n    - offline_access\n  dynamic_client_registration: true\n  protected_resource_metadata: well-known/lev-oauth-protected-resource.json\nrequired_headers:\n- name: Authorization\n  value: Bearer <token>\n  required: true\n- name: X-Origin-App\n  value: <client-name>\n  required: true\n  description: Identifies the calling application (for example \"my-integration\").\n- name: X-Active-Account\n  value: <account-slug>\n  required: false\n  description: Required only for JWT users with active memberships on more than one\n    account. Not applicable to API keys, which are account-bound.\npermission_levels:\n- name: full_access\n  default: true\n  description: All scopes granted to the key.\n- name: read_only\n  default: false\n  description: Read scopes only.\nerrors:\n- status: 401\n  type: unauthorized\n  meaning: Missing, invalid, or\
  \ expired token.\n- status: 403\n  type: forbidden\n  meaning: Valid token but insufficient permissions for the resource.\nrelated:\n  scopes: scopes/lev-scopes.yml\n  conventions: conventions/lev-conventions.yml\n  well_known: well-known/lev-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lev/refs/heads/main/authentication/lev-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Commercial Real Estate
- Real Estate
- Proptech
- CRE Financing
- Lending
- CRM
- Artificial Intelligence
- AI Agents
- Deal Management
- Market Data
- Documents
---
