---
anonymous_access: false
api_key_in: []
api_specs:
- filename: savee-boards-api-openapi.yml
  format: yaml
  label: Savee Boards API
  slug: savee-boards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/savee/refs/heads/main/openapi/savee-boards-api-openapi.yml
- filename: savee-saves-api-openapi.yml
  format: yaml
  label: Savee Saves API
  slug: savee-saves-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/savee/refs/heads/main/openapi/savee-saves-api-openapi.yml
- filename: savee-search-api-openapi.yml
  format: yaml
  label: Savee Search API
  slug: savee-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/savee/refs/heads/main/openapi/savee-search-api-openapi.yml
- filename: savee-system-api-openapi.yml
  format: yaml
  label: Savee System API
  slug: savee-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/savee/refs/heads/main/openapi/savee-system-api-openapi.yml
- filename: savee-user-api-openapi.yml
  format: yaml
  label: Savee User API
  slug: savee-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/savee/refs/heads/main/openapi/savee-user-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Savee Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Savee secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Savee
provider_slug: savee
scheme_count: 2
schemes:
- bearerFormat: sv_live_…
  description: '**Personal access token** (`sv_live_…`) — represents you and carries every scope, so no scope is required for this call. Best for your own scripts and internal tools. Generate one at https://savee.com/developers/.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/savee-boards-api-openapi.yml
  - openapi/savee-saves-api-openapi.yml
  - openapi/savee-search-api-openapi.yml
  - openapi/savee-user-api-openapi.yml
  type: http
- description: '**OAuth access token** (`sv_at_…`) — obtained on one of your users’ behalf and limited to the scopes they approved. Use this when you’re building a product other people sign into with Savee. See https://docs.savee.com/api/oauth.


    Missing the scope below returns `403` with a `WWW-Authenticate: Bearer error="insufficient_scope"` header naming it.'
  flows:
  - authorizationUrl: https://savee.com/oauth/authorize/
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://savee.com/api/oauth/token/
  name: OAuth2
  sources:
  - openapi/savee-boards-api-openapi.yml
  - openapi/savee-saves-api-openapi.yml
  - openapi/savee-search-api-openapi.yml
  - openapi/savee-user-api-openapi.yml
  type: oauth2
slug: savee-authentication
source_filename: savee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: searched\nsource: openapi/savee-boards-api-openapi.yml, openapi/savee-saves-api-openapi.yml, openapi/savee-search-api-openapi.yml,\n  openapi/savee-user-api-openapi.yml + https://docs.savee.com/api/authentication + https://docs.savee.com/api/oauth\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: sv_live_…\n  description: '**Personal access token** (`sv_live_…`) — represents you and carries every scope, so no\n    scope is required for this call. Best for your own scripts and internal tools. Generate one at https://savee.com/developers/.'\n  sources:\n  - openapi/savee-boards-api-openapi.yml\n  - openapi/savee-saves-api-openapi.yml\n  - openapi/savee-search-api-openapi.yml\n  - openapi/savee-user-api-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://savee.com/oauth/authorize/\n\
  \    tokenUrl: https://savee.com/api/oauth/token/\n    scopes: 4\n  description: |-\n    **OAuth access token** (`sv_at_…`) — obtained on one of your users’ behalf and limited to the scopes they approved. Use this when you’re building a product other people sign into with Savee. See https://docs.savee.com/api/oauth.\n\n    Missing the scope below returns `403` with a `WWW-Authenticate: Bearer error=\"insufficient_scope\"` header naming it.\n  sources:\n  - openapi/savee-boards-api-openapi.yml\n  - openapi/savee-saves-api-openapi.yml\n  - openapi/savee-search-api-openapi.yml\n  - openapi/savee-user-api-openapi.yml\ndocs: https://docs.savee.com/api/authentication\ndetails:\n  personal_access_token:\n    format: sv_live_ prefix followed by 24 characters\n    issuance: Savee → Settings → Developers → API Access; shown once, SHA-256 hash stored\n    concurrency: At most one active token per user; generating a new one revokes the previous\n    expiry: None — revoked by regenerate/revoke, or\
  \ rejected with 402 while the subscription is lapsed\n    scope: Carries every scope implicitly\n  oauth:\n    access_token: sv_at_ prefix; 1-hour lifetime (expires_in 3600)\n    refresh_token: sv_rt_ prefix; 30-day lifetime, rotates on every use; replaying a used refresh token\n      revokes the entire chain\n    client_type: Confidential — client secret required at the token endpoint (client_secret_basic or client_secret_post)\n    pkce: S256 required; plain rejected\n    resource_indicator: resource=https://api.savee.com required on authorization and token requests (RFC\n      8707)\n    registration: Invite-only while partner integrations are onboarded one at a time (hey@savee.com);\n      up to 6 apps and 10 redirect URLs per account, exact-match https redirects (http only on localhost)\n    metadata: https://savee.com/.well-known/oauth-authorization-server (RFC 8414, probed 200 on 2026-09-03)\n    revocation: https://savee.com/api/oauth/revoke/ (RFC 7009)\n  subscription_gate: Both\
  \ token types require an active paid Savee subscription, checked on every request\n    — 402 PAYMENT_REQUIRED when lapsed\n  cors: 'Access-Control-Allow-Origin: * is sent, with explicit guidance never to ship tokens to browsers'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/savee/refs/heads/main/authentication/savee-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Design
- visual inspiration
- Image
- Creative
- Moodboards
- Artificial Intelligence (AI)
---
