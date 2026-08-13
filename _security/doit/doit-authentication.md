---
api_key_in:
- header
api_specs:
- filename: doit-openapi-original.yml
  format: yaml
  label: DoiT API
  slug: doit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doit/refs/heads/main/openapi/doit-openapi-original.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Doit Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: DoiT secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: DoiT
provider_slug: doit
scheme_count: 3
schemes:
- description: Use the "Bearer <API_KEY>" format or sign in for autofill
  format: Bearer <API_TOKEN>
  in: header
  name: api_key
  parameter: Authorization
  sources:
  - openapi/doit-openapi-original.yml
  token_types:
  - best_for: Scripts, local tools, or automation tied to your user
    create_at: https://app.doit.com/profile/api
    name: Personal API token
    scope: Limited to the permissions the creating user's role already grants; effective permissions narrow if that role changes.
    status: current
  - best_for: Shared automation (CI/CD, scheduled jobs, integrations) that must not depend on one person
    create_at: DoiT console → Users and access → Service accounts → API tokens
    name: Service account API token
    scope: Uses the service account's current permissions; changes take effect immediately and removed permissions cause 403 on affected endpoints. Service accounts have no user email, so private user-only Cloud Analytics reports are unreachable — reports must be shared organization-wide or be preset reports.
    status: current
  - name: Legacy API token
    note: Existing legacy tokens keep working until revoked and reflect the user's current role permissions. Creating new legacy tokens is deprecated. Only legacy keys honour the customerContext query parameter.
    status: deprecated
  type: apiKey
- description: Tenant (customer) ID that sets the request's customer context. Required when the credential can access more than one tenant; omit when the credential is scoped to exactly one tenant. Omitting it for a multi-tenant credential fails with 400 / tenant_id_required; conflicting with the credential's tenant scope fails with 400 / tenant_id_mismatch. Supersedes the legacy customerContext query parameter.
  in: header
  name: tenantId
  parameter: X-Tenant-Id
  sources:
  - openapi/doit-openapi-original.yml
  type: apiKey
- discovery: https://console.doit.com/.well-known/oauth-authorization-server
  dynamic_client_registration: https://console.doit.com/api/oauth/register
  flows:
  - authorizationUrl: https://console.doit.com/sign-in/oauth
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://console.doit.com/api/auth/token
  jwks: https://console.doit.com/.well-known/jwks.json
  name: oauth2
  pkce: S256
  revocation: https://console.doit.com/api/oauth/revoke
  sources:
  - openapi/doit-openapi-original.yml
  - https://console.doit.com/.well-known/oauth-authorization-server
  type: oauth2
  used_by:
  - dci CLI (dci login)
  - DoiT MCP server remote Streamable HTTP transport
slug: doit-authentication
source_filename: doit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: openapi/doit-openapi-original.yml\ndocs:\n- https://developer.doit.com/docs/start\n- https://help.doit.com/docs/general/profile/api-tokens\n- https://help.doit.com/docs/cli\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  primary: HTTP bearer token in the Authorization header\n  console: https://app.doit.com/profile/api\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: Bearer <API_TOKEN>\n  description: Use the \"Bearer <API_KEY>\" format or sign in for autofill\n  sources:\n  - openapi/doit-openapi-original.yml\n  token_types:\n  - name: Personal API token\n    status: current\n    scope: Limited to the permissions the creating user's role already grants; effective\n      permissions narrow if that role changes.\n    create_at: https://app.doit.com/profile/api\n    best_for: Scripts, local tools, or automation tied\
  \ to your user\n  - name: Service account API token\n    status: current\n    scope: Uses the service account's current permissions; changes take effect immediately\n      and removed permissions cause 403 on affected endpoints. Service accounts have\n      no user email, so private user-only Cloud Analytics reports are unreachable — reports\n      must be shared organization-wide or be preset reports.\n    create_at: DoiT console → Users and access → Service accounts → API tokens\n    best_for: Shared automation (CI/CD, scheduled jobs, integrations) that must not depend\n      on one person\n  - name: Legacy API token\n    status: deprecated\n    note: Existing legacy tokens keep working until revoked and reflect the user's current\n      role permissions. Creating new legacy tokens is deprecated. Only legacy keys honour\n      the customerContext query parameter.\n- name: tenantId\n  type: apiKey\n  in: header\n  parameter: X-Tenant-Id\n  description: Tenant (customer) ID that sets the\
  \ request's customer context. Required\n    when the credential can access more than one tenant; omit when the credential is\n    scoped to exactly one tenant. Omitting it for a multi-tenant credential fails with\n    400 / tenant_id_required; conflicting with the credential's tenant scope fails with\n    400 / tenant_id_mismatch. Supersedes the legacy customerContext query parameter.\n  sources:\n  - openapi/doit-openapi-original.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://console.doit.com/sign-in/oauth\n    tokenUrl: https://console.doit.com/api/auth/token\n    scopes: 1\n  discovery: https://console.doit.com/.well-known/oauth-authorization-server\n  pkce: S256\n  dynamic_client_registration: https://console.doit.com/api/oauth/register\n  revocation: https://console.doit.com/api/oauth/revoke\n  jwks: https://console.doit.com/.well-known/jwks.json\n  used_by:\n  - dci CLI (dci login)\n  - DoiT MCP server remote Streamable HTTP\
  \ transport\n  sources:\n  - openapi/doit-openapi-original.yml\n  - https://console.doit.com/.well-known/oauth-authorization-server\nmcp_authentication:\n  resource: https://mcp.doit.com\n  metadata: https://mcp.doit.com/.well-known/oauth-protected-resource\n  challenge: 'WWW-Authenticate: Bearer resource_metadata=\"https://mcp.doit.com/.well-known/oauth-protected-resource\",\n    error=\"invalid_token\" (observed on an unauthenticated tools/list, HTTP 401)'\n  scopes:\n  - mcp:tools\n  - mcp:resources\n  - offline_access\n  stdio_alternative: DOIT_API_KEY environment variable holding a personal API token (no\n    browser flow)\nsecurity_guidance:\n  storage: DoiT instructs treating API tokens like passwords — store in a secrets manager\n    or CI/CD secret store, never commit to source control or share in chat.\n  sops: https://developer.doit.com/docs/managing-the-api-token-with-sops\nobserved_unauthenticated_response:\n  url: https://api.doit.com/analytics/v1/reports\n  http_status:\
  \ 401\n  body: '{\"error\":\"no Authorization header\"}'\n  fetched: '2026-08-12'\nscopes_artifact: scopes/doit-scopes.yml\nx-evidence:\n- url: https://developer.doit.com/docs/start\n  http_status: 200\n  fetched: '2026-08-12'\n- url: https://api.doit.com/openapi.yaml\n  http_status: 200\n  fetched: '2026-08-12'\n- url: https://mcp.doit.com/mcp\n  http_status: 401\n  fetched: '2026-08-12'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doit/refs/heads/main/authentication/doit-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Company
- FinOps
- Cloud Cost Management
- Cloud Intelligence
- Cost Optimization
- Multicloud
- Kubernetes
- Analytics
- MCP
- Artificial Intelligence
---
