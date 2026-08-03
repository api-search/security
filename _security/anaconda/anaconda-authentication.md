---
api_key_in:
- header
api_specs:
- filename: anaconda-server-openapi-original.json
  format: json
  label: Anaconda Server API
  slug: server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anaconda/refs/heads/main/openapi/anaconda-server-openapi-original.json
- filename: anaconda-org-management-openapi-original.json
  format: json
  label: Anaconda Organization Management API
  slug: org-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anaconda/refs/heads/main/openapi/anaconda-org-management-openapi-original.json
- filename: anaconda-audit-logs-openapi-original.json
  format: json
  label: Anaconda Audit Logs API
  slug: audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anaconda/refs/heads/main/openapi/anaconda-audit-logs-openapi-original.json
- filename: anaconda-ai-navigator-openapi-original.json
  format: json
  label: Anaconda AI Navigator API
  slug: ai-navigator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anaconda/refs/heads/main/openapi/anaconda-ai-navigator-openapi-original.json
- filename: anaconda-desktop-openapi-original.json
  format: json
  label: Anaconda Desktop API
  slug: desktop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anaconda/refs/heads/main/openapi/anaconda-desktop-openapi-original.json
auth_types:
- http
- apiKey
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Anaconda Authentication
name_suffix: Authentication
oauth_flows:
- authorization_code
- client_credentials
- refresh_token
- password
- device_code
overview: Anaconda secures its APIs with http, apiKey, and openIdConnect across 6 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorization_code, client_credentials, refresh_token, password, and device_code flow(s).
provider_name: Anaconda
provider_slug: anaconda
scheme_count: 6
schemes:
- bearerFormat: JWT
  description: Bearer token obtained by authenticating with an organization service account's client_id and client_secret.
  name: JWT or Access Token
  scheme: bearer
  sources:
  - openapi/anaconda-org-management-openapi-original.json
  - openapi/anaconda-audit-logs-openapi-original.json
  type: http
- bearerFormat: JWT
  description: Bearer token obtained by authenticating with an organization admin's email and password (grant_type=password).
  name: Organization Admin
  scheme: bearer
  sources:
  - openapi/anaconda-org-management-openapi-original.json
  type: http
- bearerFormat: JWT
  description: Anaconda Server / Anaconda Platform repository API bearer token.
  name: jwt
  scheme: bearer
  sources:
  - openapi/anaconda-server-openapi-original.json
  type: http
- description: Long-lived user private token for the Anaconda Server repository API, sent in the X-Auth header. This is the token class `anaconda token install` provisions for conda clients.
  in: header
  name: user_token
  parameter: X-Auth
  sources:
  - openapi/anaconda-server-openapi-original.json
  type: apiKey
- bearerFormat: UUID
  description: API key for the local Desktop and AI Navigator APIs ("Enter your API key here").
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/anaconda-desktop-openapi-original.json
  - openapi/anaconda-ai-navigator-openapi-original.json
  type: http
- description: Anaconda.org repository token, created with `anaconda org auth --create` or in the anaconda.org UI. Anonymous reads are permitted; writes and private-channel reads require a token. Not declared in any OpenAPI — captured from the docs.
  in: header
  name: anaconda.org token
  parameter: Authorization
  sources:
  - https://anaconda.com/docs/anaconda-org/admin-guide/tokens
  type: apiKey
slug: anaconda-authentication
source_filename: anaconda-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: openapi/anaconda-ai-navigator-openapi-original.json, openapi/anaconda-audit-logs-openapi-original.json,\n  openapi/anaconda-desktop-openapi-original.json, openapi/anaconda-org-management-openapi-original.json,\n  openapi/anaconda-server-openapi-original.json, well-known/anaconda-openid-configuration.json\ndocs: https://anaconda.com/docs/anaconda-platform/user/api-keys\ndocs_additional:\n- https://anaconda.com/docs/anaconda-platform/admin/audit-logs/audit-log-api\n- https://anaconda.com/docs/anaconda-platform/admin/org-management-api/org-management-api\n- https://anaconda.com/docs/cli-reference/anaconda-auth/getting-started\n- https://anaconda.com/docs/anaconda-org/admin-guide/tokens\nsummary:\n  types:\n  - http\n  - apiKey\n  - openIdConnect\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - password\n  - device_code\n  note: Anaconda runs a single OIDC identity\
  \ service (issuer https://auth.anaconda.com/api/auth)\n    that mints the bearer tokens the Platform APIs accept. The individual OpenAPI documents\n    declare only the bearer/apiKey schemes; the OAuth 2.0 / OIDC layer is discovered\n    from /.well-known/openid-configuration and documented in the docs pages above.\nidentity_provider:\n  issuer: https://auth.anaconda.com/api/auth\n  discovery: https://anaconda.com/.well-known/openid-configuration\n  file: well-known/anaconda-openid-configuration.json\n  authorization_endpoint: https://anaconda.com/api/auth/oauth2/authorize\n  token_endpoint: https://anaconda.com/api/auth/oauth2/token\n  device_authorization_endpoint: https://anaconda.com/api/auth/oauth2/device/authorize\n  userinfo_endpoint: https://anaconda.com/api/auth/oauth2/userinfo\n  end_session_endpoint: https://anaconda.com/api/auth/oauth2/sessions/logout\n  jwks_uri: https://anaconda.com/api/auth/.well-known/jwks.json\n  scopes_supported:\n  - openid\n  - profile\n  - email\n\
  \  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - client_credentials\n  - password\n  - urn:ietf:params:oauth:grant-type:device_code\n  response_types_supported:\n  - code\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\nservice_account_flow:\n  description: Machine-to-machine access for the Organization Management API and the\n    Audit Logs API. Create a service account in the Anaconda Platform admin console,\n    then exchange its client_id/client_secret for a short-lived bearer token.\n  token_endpoint: https://anaconda.com/api/iam/token\n  grant_type: client_credentials\n  content_type: application/x-www-form-urlencoded\n  token_type: Bearer\n  expires_in: 900\n  required_headers:\n  - name: Authorization\n    value: Bearer <ACCESS_TOKEN>\n  - name: X-Org-Name\n    value: <ORG_ID>\n  - name: X-API-Version\n    value: v1\n  docs: https://anaconda.com/docs/anaconda-platform/admin/audit-logs/audit-log-api\nschemes:\n\
  - name: JWT or Access Token\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token obtained by authenticating with an organization service\n    account's client_id and client_secret.\n  sources:\n  - openapi/anaconda-org-management-openapi-original.json\n  - openapi/anaconda-audit-logs-openapi-original.json\n- name: Organization Admin\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token obtained by authenticating with an organization admin's\n    email and password (grant_type=password).\n  sources:\n  - openapi/anaconda-org-management-openapi-original.json\n- name: jwt\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Anaconda Server / Anaconda Platform repository API bearer token.\n  sources:\n  - openapi/anaconda-server-openapi-original.json\n- name: user_token\n  type: apiKey\n  in: header\n  parameter: X-Auth\n  description: Long-lived user private token for the Anaconda Server repository API,\n    sent in\
  \ the X-Auth header. This is the token class `anaconda token install` provisions\n    for conda clients.\n  sources:\n  - openapi/anaconda-server-openapi-original.json\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: UUID\n  description: 'API key for the local Desktop and AI Navigator APIs (\"Enter your API\n    key here\").'\n  sources:\n  - openapi/anaconda-desktop-openapi-original.json\n  - openapi/anaconda-ai-navigator-openapi-original.json\n- name: anaconda.org token\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Anaconda.org repository token, created with `anaconda org auth --create`\n    or in the anaconda.org UI. Anonymous reads are permitted; writes and private-channel\n    reads require a token. Not declared in any OpenAPI — captured from the docs.'\n  sources:\n  - https://anaconda.com/docs/anaconda-org/admin-guide/tokens\nx-evidence:\n  fetched: '2026-08-02'\n  openid_configuration_http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anaconda/refs/heads/main/authentication/anaconda-authentication.yml
summary_line: http/apiKey/openIdConnect · 6 schemes
tags:
- Company
- Data Science
- Machine Learning
- Artificial Intelligence
- Package Management
- Python
- Developer Tools
- Software Supply Chain
- Repository
- Package Registry
- Conda
- MCP
---
