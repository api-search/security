---
anonymous_access: false
api_key_in:
- cookie
api_specs:
- filename: cliponit-app-account-api-openapi.yml
  format: yaml
  label: ClipOnIt Account API
  slug: cliponit-app-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cliponit-app/openapi/cliponit-app-account-api-openapi.yml
- filename: cliponit-app-agents-api-openapi.yml
  format: yaml
  label: ClipOnIt Agents API
  slug: cliponit-app-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cliponit-app/openapi/cliponit-app-agents-api-openapi.yml
- filename: cliponit-app-auth-api-openapi.yml
  format: yaml
  label: ClipOnIt Auth API
  slug: cliponit-app-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cliponit-app/openapi/cliponit-app-auth-api-openapi.yml
- filename: cliponit-app-billing-api-openapi.yml
  format: yaml
  label: ClipOnIt Billing API
  slug: cliponit-app-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cliponit-app/openapi/cliponit-app-billing-api-openapi.yml
- filename: cliponit-app-clips-api-openapi.yml
  format: yaml
  label: ClipOnIt Clips API
  slug: cliponit-app-clips-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cliponit-app/openapi/cliponit-app-clips-api-openapi.yml
- filename: cliponit-app-enrich-api-openapi.yml
  format: yaml
  label: ClipOnIt Enrich API
  slug: cliponit-app-enrich-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cliponit-app/openapi/cliponit-app-enrich-api-openapi.yml
- filename: cliponit-app-explainer-api-openapi.yml
  format: yaml
  label: ClipOnIt Explainer API
  slug: cliponit-app-explainer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cliponit-app/openapi/cliponit-app-explainer-api-openapi.yml
- filename: cliponit-app-smart-api-openapi.yml
  format: yaml
  label: ClipOnIt Smart API
  slug: cliponit-app-smart-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cliponit-app/openapi/cliponit-app-smart-api-openapi.yml
- filename: cliponit-app-tiktok-api-openapi.yml
  format: yaml
  label: ClipOnIt Tiktok API
  slug: cliponit-app-tiktok-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cliponit-app/openapi/cliponit-app-tiktok-api-openapi.yml
- filename: cliponit-app-videos-api-openapi.yml
  format: yaml
  label: ClipOnIt Videos API
  slug: cliponit-app-videos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cliponit-app/openapi/cliponit-app-videos-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: ClipOnIt Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: ClipOnIt secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: ClipOnIt
provider_slug: cliponit-app
scheme_count: 3
schemes:
- bearerFormat: ck_<64 hex>
  description: 'Personal API key from `POST /api/me/api-key` (Starter plan and above). Also accepted: the session `token` returned by `login`/`register`. Send `Authorization: Bearer ck_…`.'
  name: ApiKey
  scheme: bearer
  sources:
  - openapi/cliponit-app-openapi.yml
  type: http
- description: HttpOnly cookie set by `register`/`login` (browser clients).
  in: cookie
  name: SessionCookie
  parameter: session
  sources:
  - openapi/cliponit-app-openapi.yml
  type: apiKey
- description: 'OAuth 2.1 for MCP connectors (Claude.ai / Claude Desktop / Claude Code / ChatGPT): discovery at `/.well-known/oauth-protected-resource` and `/.well-known/oauth-authorization-server`, dynamic client registration (RFC 7591) at `/oauth/register`, PKCE S256 required, public clients only. Access tokens (`cko_…`, 1 h) are accepted everywhere a `ck_…` key is; refresh tokens (`ckr_…`, 90 days) rotate on u'
  flows:
  - authorizationUrl: https://cliponit.app/oauth/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://cliponit.app/oauth/token
  name: OAuth2
  sources:
  - openapi/cliponit-app-openapi.yml
  type: oauth2
slug: cliponit-app-authentication
source_filename: cliponit-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/cliponit-app-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - cookie\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: ApiKey\n  type: http\n  scheme: bearer\n  bearerFormat: ck_<64 hex>\n  description: 'Personal API key from `POST /api/me/api-key` (Starter plan and above). Also\n    accepted: the session `token` returned by `login`/`register`. Send `Authorization: Bearer\n    ck_…`.'\n  sources:\n  - openapi/cliponit-app-openapi.yml\n- name: SessionCookie\n  type: apiKey\n  in: cookie\n  parameter: session\n  description: HttpOnly cookie set by `register`/`login` (browser clients).\n  sources:\n  - openapi/cliponit-app-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://cliponit.app/oauth/authorize\n    tokenUrl: https://cliponit.app/oauth/token\n    scopes: 1\n  description: 'OAuth 2.1 for MCP connectors (Claude.ai\
  \ / Claude Desktop / Claude Code / ChatGPT):\n    discovery at `/.well-known/oauth-protected-resource` and `/.well-known/oauth-authorization-server`,\n    dynamic client registration (RFC 7591) at `/oauth/register`, PKCE S256 required, public\n    clients only. Access tokens (`cko_…`, 1 h) are accepted everywhere a `ck_…` key is; refresh\n    tokens (`ckr_…`, 90 days) rotate on u'\n  sources:\n  - openapi/cliponit-app-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/cliponit-app/authentication/cliponit-app-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Company
- Video
- Artificial Intelligence
- Short-Form Video
- Video Editing
- MCP
- Content Creation
- Social Media
---
