---
anonymous_access: false
api_key_in: []
api_specs:
- filename: appsmith-applications-api-openapi.yml
  format: yaml
  label: Appsmith Applications API
  slug: appsmith-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsmith/refs/heads/main/openapi/appsmith-applications-api-openapi.yml
- filename: appsmith-datasources-api-openapi.yml
  format: yaml
  label: Appsmith Datasources API
  slug: appsmith-datasources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsmith/refs/heads/main/openapi/appsmith-datasources-api-openapi.yml
- filename: appsmith-workspaces-api-openapi.yml
  format: yaml
  label: Appsmith Workspaces API
  slug: appsmith-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsmith/refs/heads/main/openapi/appsmith-workspaces-api-openapi.yml
auth_types:
- cookie
- http-bearer
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Appsmith Authentication
name_suffix: Authentication
oauth_flows: []
overview: Appsmith secures its APIs with cookie, http-bearer, and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Appsmith
provider_slug: appsmith
scheme_count: 3
schemes:
- description: Session cookie established by the browser sign-in flow (form login, Google SSO on Free, SAML/OIDC on Enterprise). This is what the /api/v1 platform API actually authenticates. Unauthenticated calls return the anonymousUser identity (GET /api/v1/users/me -> 200 with "email":"anonymousUser") or 401.
  documented_as_public_api: false
  evidence: https://app.appsmith.com/api/v1/users/me (HTTP 200, 2026-09-04)
  in: cookie
  name: editorSession
  surface: https://app.appsmith.com/api/v1
  type: cookie
- description: Per-user MCP bearer token created at Profile -> MCP tokens. Every tool call it authorizes stays bounded by that user's own ACL. Rejected with 401 and non-creatable while APPSMITH_MCP_ENABLED is off; authentication attempts are throttled to 5 per minute.
  name: mcpToken
  prefix: mcp_
  scheme: bearer
  source: https://github.com/appsmithorg/appsmith/blob/release/app/client/packages/mcp/README.md
  surface: https://{your-appsmith-instance}/mcp
  type: http
- description: API key generated in the Appsmith admin UI ("API key to setup SCIM") and configured in the identity provider for SCIM 2.0 user and group provisioning. Enterprise plan.
  header: Authorization
  in: header
  name: scimApiKey
  source: https://docs.appsmith.com/advanced-concepts/user-provisioning-group-sync
  surface: https://{your-domain}/scim
  type: apiKey
slug: appsmith-authentication
source_filename: appsmith-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: https://docs.appsmith.com + appsmithorg/appsmith source + live probes of https://app.appsmith.com/api/v1\nname: Appsmith authentication\nnote: 'Upgraded from a derived profile that read a single bearerAuth scheme out of the scaffold OpenAPI in this repository.\n  Appsmith has no general-purpose REST API key: there are three distinct credential kinds, each scoped to a different\n  surface.'\nsummary:\n  types:\n  - cookie\n  - http-bearer\n  - apiKey\n  public_api_key: false\nschemes:\n- name: editorSession\n  type: cookie\n  in: cookie\n  surface: https://app.appsmith.com/api/v1\n  description: Session cookie established by the browser sign-in flow (form login, Google SSO on Free, SAML/OIDC on\n    Enterprise). This is what the /api/v1 platform API actually authenticates. Unauthenticated calls return the anonymousUser\n    identity (GET /api/v1/users/me -> 200 with \"email\":\"anonymousUser\") or 401.\n  documented_as_public_api:\
  \ false\n  evidence: https://app.appsmith.com/api/v1/users/me (HTTP 200, 2026-09-04)\n- name: mcpToken\n  type: http\n  scheme: bearer\n  prefix: mcp_\n  surface: https://{your-appsmith-instance}/mcp\n  description: Per-user MCP bearer token created at Profile -> MCP tokens. Every tool call it authorizes stays bounded\n    by that user's own ACL. Rejected with 401 and non-creatable while APPSMITH_MCP_ENABLED is off; authentication\n    attempts are throttled to 5 per minute.\n  source: https://github.com/appsmithorg/appsmith/blob/release/app/client/packages/mcp/README.md\n- name: scimApiKey\n  type: apiKey\n  in: header\n  header: Authorization\n  surface: https://{your-domain}/scim\n  description: API key generated in the Appsmith admin UI (\"API key to setup SCIM\") and configured in the identity\n    provider for SCIM 2.0 user and group provisioning. Enterprise plan.\n  source: https://docs.appsmith.com/advanced-concepts/user-provisioning-group-sync\ninstance_sso:\n  free:\n  - Google\
  \ SSO\n  enterprise:\n  - SAML 2.0\n  - OIDC\n  source: https://www.appsmith.com/pricing\n  recovery: appsmithctl enable-form-login re-enables email/password sign-in if SSO configuration locks an instance\n    out.\ndatasource_auth:\n  note: 'Distinct from platform auth: Appsmith CONSUMES auth on behalf of apps — Authenticated API datasources support\n    API keys, bearer tokens, basic auth and OAuth 2.0, with credentials stored server-side rather than in the app\n    definition.'\n  source: https://docs.appsmith.com/connect-data/reference/authenticated-api\noauth_scopes:\n  published: false\n  note: Appsmith is an OAuth relying party, not an authorization server; there is no scope surface to document.\nevidence:\n- url: https://app.appsmith.com/api/v1/users/me\n  http_status: 200\n- url: https://app.appsmith.com/api/v1/workspaces\n  http_status: 401\n- url: https://docs.appsmith.com/advanced-concepts/user-provisioning-group-sync\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appsmith/refs/heads/main/authentication/appsmith-authentication.yml
summary_line: cookie/http-bearer/apiKey · 3 schemes
tags:
- Low-Code
- Open-Source
- Internal Tools
- Workflow-Automation
- Developer Tools
---
