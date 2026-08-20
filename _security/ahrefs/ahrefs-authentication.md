---
api_key_in: []
api_specs:
- filename: ahrefs-openapi-original.json
  format: json
  label: Ahrefs API v3
  slug: api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahrefs/refs/heads/main/openapi/_original/ahrefs-openapi-original.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Ahrefs Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Ahrefs secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Ahrefs
provider_slug: ahrefs
scheme_count: 3
schemes:
- applied_globally: true
  format: 'Authorization: Bearer <API_KEY>'
  in: header
  name: http
  parameter: Authorization
  scheme: bearer
  source: openapi
  sources:
  - openapi/_original/ahrefs-openapi-original.json
  - openapi/ahrefs-site-explorer-openapi.json
  - openapi/ahrefs-keywords-explorer-openapi.json
  - openapi/ahrefs-site-audit-openapi.json
  - openapi/ahrefs-rank-tracker-openapi.json
  - openapi/ahrefs-serp-overview-openapi.json
  - openapi/ahrefs-batch-analysis-openapi.json
  - openapi/ahrefs-subscription-info-openapi.json
  - openapi/ahrefs-management-openapi.json
  - openapi/ahrefs-brand-radar-openapi.json
  - openapi/ahrefs-web-analytics-openapi.json
  - openapi/ahrefs-gsc-openapi.json
  - openapi/ahrefs-social-media-openapi.json
  type: http
- client_secret: web apps only; omitted for desktop apps
  docs: https://docs.ahrefs.com/ahrefs-connect/docs/oauth-guide.md
  flows:
  - authorizationUrl: https://app.ahrefs.com/web/oauth/authorize
    code_challenge_method: S256
    flow: authorizationCode
    pkce: required
    scopes:
    - apiv3-integration-apps
    tokenUrl: https://ahrefs.com/oauth/token
  name: ahrefs-connect-oauth2
  refresh_tokens: false
  source: docs
  token_lifetime: 1 year (no refresh token; user must re-authorize on expiry)
  type: oauth2
- discovery: well-known/ahrefs-oauth-authorization-server.json
  flows:
  - authorizationUrl: https://app.ahrefs.com/web/oauth/authorize
    code_challenge_method: S256
    flow: authorizationCode
    pkce: supported
    registrationUrl: https://api.ahrefs.com/mcp/register
    scopes:
    - apiv3-mcp
    tokenUrl: https://ahrefs.com/oauth/token
  grant_types:
  - implicit
  - authorization_code
  - authorization_code_with_pkce
  name: ahrefs-mcp-oauth2
  source: probed
  type: oauth2
slug: ahrefs-authentication
source_filename: ahrefs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://docs.ahrefs.com/api/docs/api-keys-creation-and-management.md\ndocs:\n- https://docs.ahrefs.com/api/docs/api-keys-creation-and-management.md\n- https://docs.ahrefs.com/ahrefs-connect/docs/oauth-guide.md\n- https://docs.ahrefs.com/mcp/docs/introduction.md\nsummary:\n  types:\n  - http\n  - oauth2\n  http_schemes:\n  - bearer\n  oauth2_flows:\n  - authorizationCode\n  oauth2_pkce: S256\n  note: >-\n    The OpenAPI declares a single `http` bearer scheme. The docs additionally describe two OAuth 2.0\n    surfaces that the spec does not model: Ahrefs Connect (partner apps, scope `apiv3-integration-apps`)\n    and the hosted MCP server (scope `apiv3-mcp`, advertised in the RFC 8414 metadata at\n    https://api.ahrefs.com/.well-known/oauth-authorization-server).\nschemes:\n- name: http\n  type: http\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  format: 'Authorization: Bearer <API_KEY>'\n  source: openapi\n\
  \  applied_globally: true\n  sources:\n  - openapi/_original/ahrefs-openapi-original.json\n  - openapi/ahrefs-site-explorer-openapi.json\n  - openapi/ahrefs-keywords-explorer-openapi.json\n  - openapi/ahrefs-site-audit-openapi.json\n  - openapi/ahrefs-rank-tracker-openapi.json\n  - openapi/ahrefs-serp-overview-openapi.json\n  - openapi/ahrefs-batch-analysis-openapi.json\n  - openapi/ahrefs-subscription-info-openapi.json\n  - openapi/ahrefs-management-openapi.json\n  - openapi/ahrefs-brand-radar-openapi.json\n  - openapi/ahrefs-web-analytics-openapi.json\n  - openapi/ahrefs-gsc-openapi.json\n  - openapi/ahrefs-social-media-openapi.json\n- name: ahrefs-connect-oauth2\n  type: oauth2\n  source: docs\n  docs: https://docs.ahrefs.com/ahrefs-connect/docs/oauth-guide.md\n  flows:\n  - flow: authorizationCode\n    pkce: required\n    code_challenge_method: S256\n    authorizationUrl: https://app.ahrefs.com/web/oauth/authorize\n    tokenUrl: https://ahrefs.com/oauth/token\n    scopes:\n    - apiv3-integration-apps\n\
  \  client_secret: web apps only; omitted for desktop apps\n  refresh_tokens: false\n  token_lifetime: 1 year (no refresh token; user must re-authorize on expiry)\n- name: ahrefs-mcp-oauth2\n  type: oauth2\n  source: probed\n  discovery: well-known/ahrefs-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    pkce: supported\n    code_challenge_method: S256\n    authorizationUrl: https://app.ahrefs.com/web/oauth/authorize\n    tokenUrl: https://ahrefs.com/oauth/token\n    registrationUrl: https://api.ahrefs.com/mcp/register\n    scopes:\n    - apiv3-mcp\n  grant_types:\n  - implicit\n  - authorization_code\n  - authorization_code_with_pkce\napi_keys:\n  create_at: https://app.ahrefs.com/account/api-keys\n  who_can_create: workspace owners and admins only\n  max_keys: 1000\n  key_lifetime: 1 year, after which the key expires and becomes inactive\n  revocation: a key is invalidated when the user who created it is removed from the workspace\n  usage_controls: per-key monthly\
  \ API-unit limits, plus a workspace-level pay-as-you-go cap\npublic_endpoints:\n  note: >-\n    The `Public` tool (crawler IP addresses/ranges and free domain rating) is documented as usable\n    without an Ahrefs subscription; a free/public APIv3 key may still be required for some of them.\n  spec: openapi/ahrefs-public-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ahrefs/refs/heads/main/authentication/ahrefs-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- SEO
- Marketing
- Search
- Analytics
- Backlinks
- Keywords
- Web Analytics
- Rank Tracking
- Site Audit
- Brand Monitoring
- Social-Media
---
