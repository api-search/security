---
api_key_in:
- header
api_specs:
- filename: index.html
  format: yaml
  label: Skyvia Public API
  slug: skyvia-public-api
  spec_type: OpenAPI
  url: https://api.skyvia.com/swagger/index.html
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Skyvia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Skyvia secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Skyvia
provider_slug: skyvia
scheme_count: 2
schemes:
- description: Authorization header with the Skyvia access token.
  expiry:
    max_lifetime: 1 year
    note: '"you cannot create token lasting longer than a year." Tokens display an expiration date and a last-used timestamp in Account Settings > API Settings.'
  in: header
  issuance: Self-service in the Skyvia app under Account Settings > API Settings.
  name: Access Token
  observed_failure:
    body: '{"errorCode":403,"errors":{},"message":"Authorization header is missing or invalid.","refresh":false}'
    http_status: 403
    note: Probed live and unauthenticated on 2026-08-12. Skyvia answers a missing or invalid token with 403, not 401, and returns no WWW-Authenticate challenge — so a client cannot discover the scheme from the response. The spec declares no 401/403 response at all, so this envelope is undocumented.
  parameter: Authorization
  rotation: Manual — create a new token and delete the old one; no programmatic rotation endpoint exists.
  scoped: true
  scopes: scopes/skyvia-scopes.yml
  sources:
  - openapi/skyvia-account-api-openapi.yml
  - openapi/skyvia-agents-api-openapi.yml
  - openapi/skyvia-automations-api-openapi.yml
  - openapi/skyvia-backups-api-openapi.yml
  - openapi/skyvia-connections-api-openapi.yml
  - openapi/skyvia-endpoints-api-openapi.yml
  - openapi/skyvia-integrations-api-openapi.yml
  - openapi/skyvia-workspaces-api-openapi.yml
  surface: Skyvia Public API (https://api.skyvia.com)
  type: apiKey
- additional_controls:
  - IP address filtering (allow-list of ranges permitted to reach the endpoint)
  - Per-object and per-operation permissions on the endpoint
  description: Per-endpoint user accounts. Credentials are the endpoint user name and password joined with a colon and base64-encoded into the Authorization header. Security is optional per endpoint — an endpoint with no user accounts is reachable by anyone holding the endpoint URL, which is what makes an MCP endpoint usable from the Claude web client. Adding user accounts restricts the endpoint to clients that support authenticated MCP, such as Claude Desktop.
  docs: https://docs.skyvia.com/connect/security-settings.html
  name: Connect endpoint user
  optional: true
  scheme: basic
  sources:
  - https://docs.skyvia.com/connect/security-settings.html
  - https://docs.skyvia.com/connect/mcp-endpoints/using-with-claude.html
  surface: Skyvia Connect OData / SQL / MCP endpoints
  type: http
slug: skyvia-authentication
source_filename: skyvia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: openapi/*.yml (derived baseline) + https://docs.skyvia.com/account-management/api-settings.html\ndocs: https://docs.skyvia.com/account-management/api-settings.html\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  oauth2_flows: []\n  note: >-\n    Skyvia uses no OAuth 2.0 and no OpenID Connect on any of its own surfaces. The Public REST API is\n    authenticated with a single opaque, scoped, expiring API token in the Authorization header. Skyvia\n    Connect endpoints (OData, SQL, MCP) use a separate, per-endpoint credential model — optional HTTP Basic\n    endpoint users plus an IP allow-list — which is unrelated to the account API token.\nschemes:\n- name: Access Token\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Authorization header with the Skyvia access token.\n  surface: Skyvia Public API (https://api.skyvia.com)\n  scoped: true\n  scopes: scopes/skyvia-scopes.yml\n \
  \ expiry:\n    max_lifetime: 1 year\n    note: >-\n      \"you cannot create token lasting longer than a year.\" Tokens display an expiration date and a last-used\n      timestamp in Account Settings > API Settings.\n  issuance: Self-service in the Skyvia app under Account Settings > API Settings.\n  rotation: Manual — create a new token and delete the old one; no programmatic rotation endpoint exists.\n  observed_failure:\n    http_status: 403\n    body: '{\"errorCode\":403,\"errors\":{},\"message\":\"Authorization header is missing or invalid.\",\"refresh\":false}'\n    note: >-\n      Probed live and unauthenticated on 2026-08-12. Skyvia answers a missing or invalid token with 403, not\n      401, and returns no WWW-Authenticate challenge — so a client cannot discover the scheme from the\n      response. The spec declares no 401/403 response at all, so this envelope is undocumented.\n  sources:\n  - openapi/skyvia-account-api-openapi.yml\n  - openapi/skyvia-agents-api-openapi.yml\n\
  \  - openapi/skyvia-automations-api-openapi.yml\n  - openapi/skyvia-backups-api-openapi.yml\n  - openapi/skyvia-connections-api-openapi.yml\n  - openapi/skyvia-endpoints-api-openapi.yml\n  - openapi/skyvia-integrations-api-openapi.yml\n  - openapi/skyvia-workspaces-api-openapi.yml\n- name: Connect endpoint user\n  type: http\n  scheme: basic\n  surface: Skyvia Connect OData / SQL / MCP endpoints\n  optional: true\n  description: >-\n    Per-endpoint user accounts. Credentials are the endpoint user name and password joined with a colon and\n    base64-encoded into the Authorization header. Security is optional per endpoint — an endpoint with no\n    user accounts is reachable by anyone holding the endpoint URL, which is what makes an MCP endpoint usable\n    from the Claude web client. Adding user accounts restricts the endpoint to clients that support\n    authenticated MCP, such as Claude Desktop.\n  additional_controls:\n  - IP address filtering (allow-list of ranges permitted to reach\
  \ the endpoint)\n  - Per-object and per-operation permissions on the endpoint\n  docs: https://docs.skyvia.com/connect/security-settings.html\n  sources:\n  - https://docs.skyvia.com/connect/security-settings.html\n  - https://docs.skyvia.com/connect/mcp-endpoints/using-with-claude.html\naccount_level_controls:\n- control: Two-factor authentication\n  scope: Skyvia account sign-in\n  enforceable: true\n  note: An account can require all users to have 2FA enabled (added June 2026).\n  docs: https://docs.skyvia.com/profile-management/two-factor-authentication.html\n- control: IP filtering\n  scope: Skyvia account sign-in\n  note: Restricts account access to specific IP addresses (added June 2026).\n  docs: https://docs.skyvia.com/account-management/account-security.html\ngaps:\n- No OAuth 2.0 or OIDC on any Skyvia surface; no /.well-known discovery documents are served.\n- >-\n  The Authorization header VALUE format for the Public API token is not stated anywhere in the docs — the\n  reference\
  \ says only that the token \"must be passed in the Authorization header\", and the spec's scheme\n  description repeats it. Whether a `Bearer ` prefix is required is left for the caller to discover.\n- The spec declares no 401 or 403 responses, so the auth-failure contract is undocumented in the machine-readable artifact.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skyvia/refs/heads/main/authentication/skyvia-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- data-integration
- ipaas
- etl
- elt
- data-replication
- cloud-backup
- odata
- sql
- workflow-automation
- no-code
- connectors
- data-management
- mcp
- agent-native
- data-access
---
