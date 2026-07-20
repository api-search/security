---
api_key_in:
- header
api_specs:
- filename: lightfield-openapi-original.yml
  format: yaml
  label: Lightfield API
  slug: lightfield-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightfield/refs/heads/main/openapi/lightfield-openapi-original.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Lightfield Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Lightfield secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Lightfield
provider_slug: lightfield
scheme_count: 2
schemes:
- additional_required_headers:
  - error_code_when_missing: version_header
    name: Lightfield-Version
    required: true
    value: '2026-03-01'
  authorization_model: A key's access is the intersection of the scopes selected at creation and the roles of the admin who created it, evaluated at creation time.
  cli_support:
    env_var: LIGHTFIELD_API_KEY
    flag: --api-key
  docs: https://docs.lightfield.app/using-the-api/api-keys/
  failure_modes:
  - cause: Missing or invalid API key.
    status: 401
    type: unauthorized
  - cause: Valid key without the required scope for the operation.
    status: 403
    type: forbidden
  format: Bearer [example key]
  header: Authorization
  key_prefix: sk_lf_
  leaked_key_remediation: https://docs.lightfield.app/using-the-api/leaked-api-key-remediation/
  management:
    display_policy: Keys are shown once at creation and cannot be viewed again.
    revocation: immediate and permanent
    url: https://crm.lightfield.app/crm/settings/api-keys
    who_can_manage: admin users only
  name: bearerAuth
  scheme: bearer
  scope_count: 26
  scoped: true
  scopes_artifact: scopes/lightfield-scopes.yml
  sources:
  - openapi/lightfield-openapi-original.yml
  surface: rest-api
  type: http
- docs: https://docs.lightfield.app/getting-started/mcp-quickstart/
  dynamic_client_registration: true
  flows:
  - authorizationUrl: https://crm.lightfield.app/mcp/authorize
    flow: authorizationCode
    pkce:
    - S256
    refreshSupported: true
    registrationUrl: https://api.stytch.lightfield.app/v1/oauth2/register
    scopes:
      offline_access: Refresh-token issuance
      openid: OpenID Connect authentication
    tokenUrl: https://api.stytch.lightfield.app/v1/oauth2/token
  issuer: https://api.stytch.lightfield.app
  name: mcpOAuth
  resource: https://mcp.lightfield.app/mcp
  sources:
  - well-known/lightfield-oauth-authorization-server.json
  - well-known/lightfield-oauth-protected-resource.json
  spec: OAuth 2.1
  surface: mcp-server
  token_endpoint_auth_methods:
  - none
  type: oauth2
slug: lightfield-authentication
source_filename: lightfield-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/lightfield-openapi-original.yml\ndocs: https://docs.lightfield.app/using-the-api/api-keys/\nsummary:\n  types:\n  - http\n  - oauth2\n  http_schemes: [bearer]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  note: >-\n    The REST API uses a scoped bearer API key. OAuth 2.1 applies only to the hosted MCP server, not\n    to the REST surface.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  surface: rest-api\n  header: Authorization\n  format: 'Bearer [example key]'\n  key_prefix: sk_lf_\n  sources:\n  - openapi/lightfield-openapi-original.yml\n  docs: https://docs.lightfield.app/using-the-api/api-keys/\n  scoped: true\n  scopes_artifact: scopes/lightfield-scopes.yml\n  scope_count: 26\n  management:\n    url: https://crm.lightfield.app/crm/settings/api-keys\n    who_can_manage: admin users only\n    display_policy: Keys are shown once at creation and cannot be viewed again.\n    revocation:\
  \ immediate and permanent\n  authorization_model: >-\n    A key's access is the intersection of the scopes selected at creation and the roles of the admin\n    who created it, evaluated at creation time.\n  additional_required_headers:\n  - name: Lightfield-Version\n    value: '2026-03-01'\n    required: true\n    error_code_when_missing: version_header\n  failure_modes:\n  - status: 401\n    type: unauthorized\n    cause: Missing or invalid API key.\n  - status: 403\n    type: forbidden\n    cause: Valid key without the required scope for the operation.\n  cli_support:\n    env_var: LIGHTFIELD_API_KEY\n    flag: --api-key\n  leaked_key_remediation: https://docs.lightfield.app/using-the-api/leaked-api-key-remediation/\n- name: mcpOAuth\n  type: oauth2\n  surface: mcp-server\n  resource: https://mcp.lightfield.app/mcp\n  spec: OAuth 2.1\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://crm.lightfield.app/mcp/authorize\n    tokenUrl: https://api.stytch.lightfield.app/v1/oauth2/token\n\
  \    registrationUrl: https://api.stytch.lightfield.app/v1/oauth2/register\n    refreshSupported: true\n    pkce: [S256]\n    scopes:\n      openid: OpenID Connect authentication\n      offline_access: Refresh-token issuance\n  issuer: https://api.stytch.lightfield.app\n  dynamic_client_registration: true\n  token_endpoint_auth_methods: [none]\n  sources:\n  - well-known/lightfield-oauth-authorization-server.json\n  - well-known/lightfield-oauth-protected-resource.json\n  docs: https://docs.lightfield.app/getting-started/mcp-quickstart/\nsso:\n  supported: true\n  note: >-\n    Single sign-on was announced in the 2026-05-29 changelog entry; it applies to the application,\n    not to API authentication.\nbest_practices:\n- Use the narrowest scope an integration requires.\n- Never expose keys in client-side code, public repositories, or logs; use environment variables or\n  a secrets manager.\n- Use separate keys per integration so access can be revoked independently.\n- Rotate keys periodically.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightfield/refs/heads/main/authentication/lightfield-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Applications
- CRM
- Sales
- Artificial Intelligence
- Agents
- Customer Relationship Management
- Go To Market
- Productivity
- SaaS
---
