---
api_key_in: []
api_specs:
- filename: growthspace-public-api-management-openapi-original.yml
  format: yaml
  label: Growthspace Public API Management
  slug: growthspace-public-api-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/growthspace/refs/heads/main/openapi/growthspace-public-api-management-openapi-original.yml
auth_types:
- bearer-token
- client-credentials
description: ''
kind: authentication
layout: security
method: probed
name: Growthspace Authentication
name_suffix: Authentication
oauth_flows: []
overview: GrowthSpace secures its APIs with bearer-token and client-credentials across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GrowthSpace
provider_slug: growthspace
scheme_count: 1
schemes:
- credentials:
  - clientId
  - clientSecret
  name: growthspace-public-api-application
  revoke_operation: AppsManagementController_revokeApp
  scope_grant_operation: AppsManagementController_updateScopes
  scopes_source: scopes/growthspace-scopes.yml
  sources:
  - probe:/admin/apps
  - probe:/admin/apps/{appId}/token
  - probe:/public/refresh
  spec_declared: false
  token_issue_operation: AppsManagementController_generateToken
  token_refresh_operation: AppsManagementController_publicRefresh
  type: client-credentials
slug: growthspace-authentication
source_filename: growthspace-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: >-\n  https://public-api-management-dot-growthspace-246311.oa.r.appspot.com/api/docs-json\n  + https://public-api-management-dot-growthspace-246311.oa.r.appspot.com/admin/scopes\n  + the Public API Management screens in the app.growthspace.com bundle\nnote: >-\n  The published OpenAPI for the Public API Management service declares NO\n  components.securitySchemes, so nothing here is derived from a spec\n  declaration. The model below is recorded from what the service and the admin\n  console actually expose: an application is created for a company, granted a\n  subset of the 11 published scopes, and issued a clientId / clientSecret pair\n  plus a bearer token. Growthspace publishes no authentication documentation\n  page, so no docs URL can be recorded.\ndocs: null\nsummary:\n  types:\n  - bearer-token\n  - client-credentials\n  api_key_in: []\n  oauth2_flows: []\n  spec_declared_schemes: 0\n  scope_count: 11\nschemes:\n- name:\
  \ growthspace-public-api-application\n  type: client-credentials\n  spec_declared: false\n  sources:\n  - probe:/admin/apps\n  - probe:/admin/apps/{appId}/token\n  - probe:/public/refresh\n  credentials:\n  - clientId\n  - clientSecret\n  token_issue_operation: AppsManagementController_generateToken\n  token_refresh_operation: AppsManagementController_publicRefresh\n  scope_grant_operation: AppsManagementController_updateScopes\n  revoke_operation: AppsManagementController_revokeApp\n  scopes_source: scopes/growthspace-scopes.yml\nobservations:\n- observation: >-\n    GET /admin/scopes answers HTTP 200 anonymously and returns the full scope\n    catalogue. No credential was presented.\n  url: https://public-api-management-dot-growthspace-246311.oa.r.appspot.com/admin/scopes\n  http_status: 200\n- observation: >-\n    The service responds with access-control-allow-origin \"*\" and no\n    WWW-Authenticate challenge on the scope endpoint.\n  url: https://public-api-management-dot-growthspace-246311.oa.r.appspot.com/admin/scopes\n\
  \  http_status: 200\n- observation: >-\n    No /.well-known/oauth-authorization-server, /.well-known/oauth-protected-resource\n    or /.well-known/openid-configuration document is served on any Growthspace host.\n  url: https://public-api-management-dot-growthspace-246311.oa.r.appspot.com/.well-known/oauth-authorization-server\n  http_status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/growthspace/refs/heads/main/authentication/growthspace-authentication.yml
summary_line: bearer-token/client-credentials · 1 scheme
tags:
- Company
- Learning and Development
- Talent Development
- Human Resources
- Coaching
- Employee Experience
- Skills
- Workforce
- Enterprise Software
- Artificial Intelligence
---
