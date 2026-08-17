---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Markable Authentication
name_suffix: Authentication
oauth_flows: []
overview: Markable secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Markable
provider_slug: markable
scheme_count: 2
schemes:
- bearer_format: opaque access token
  credentials: email + password, submitted inside a `data` envelope
  expires: token response carries `expires_at`
  header: Authorization
  in: header
  issued_by: POST https://auth.markable.ai/auth/user/authorize
  name: userAccessToken
  scheme: bearer
  source: https://docs-dev.markable.ai/#user-authentication
  type: http
  used_for: retrieving the user record and its default client (GET https://auth.markable.ai/auth/users)
  value_form: Bearer :user_access_token
- bearer_format: opaque access token
  credentials: client_id + client_secret from the default client on the user record
  header: Authorization
  in: header
  issued_by: POST https://auth.markable.ai/auth/client/authorize
  name: clientAccessToken
  scheme: bearer
  source: https://docs-dev.markable.ai/#client-authentication
  type: http
  used_for: every Lens API call — catalog, catalog items, image search, style search, video search, taxonomy
  value_form: Bearer :client_access_token
slug: markable-authentication
source_filename: markable-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://docs-dev.markable.ai/\ndocs: https://docs-dev.markable.ai/#authentication\nnote: >-\n  Derived from the live, first-party Markable Lens API reference (Slate site served at\n  https://docs-dev.markable.ai/, source at https://github.com/markable-dev/markable-api-docs,\n  a GitHub organization whose website field is https://markable.ai). Markable publishes no\n  OpenAPI, so this profile is read from the published documentation rather than\n  securitySchemes. The authorization host (auth.markable.ai) does not currently resolve in\n  DNS — see lifecycle/markable-lifecycle.yml.\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\n  model: two-stage bearer tokens (user access token, then client access token)\n  onboarding: manual — developer signup + verification by Markable, credentials issued by\n    the vendor\nschemes:\n- name: userAccessToken\n  type: http\n  scheme: bearer\n  bearer_format: opaque access\
  \ token\n  in: header\n  header: Authorization\n  value_form: 'Bearer :user_access_token'\n  issued_by: POST https://auth.markable.ai/auth/user/authorize\n  credentials: email + password, submitted inside a `data` envelope\n  used_for: retrieving the user record and its default client (GET https://auth.markable.ai/auth/users)\n  expires: token response carries `expires_at`\n  source: https://docs-dev.markable.ai/#user-authentication\n- name: clientAccessToken\n  type: http\n  scheme: bearer\n  bearer_format: opaque access token\n  in: header\n  header: Authorization\n  value_form: 'Bearer :client_access_token'\n  issued_by: POST https://auth.markable.ai/auth/client/authorize\n  credentials: client_id + client_secret from the default client on the user record\n  used_for: every Lens API call — catalog, catalog items, image search, style search, video\n    search, taxonomy\n  source: https://docs-dev.markable.ai/#client-authentication\nreferences:\n- rfc: RFC 6750\n  what: the docs cite\
  \ HTTP Bearer Token (RFC 6750) as the authorization format\nnotes:\n- No OAuth 2.0 authorization-code/client-credentials discovery documents are published\n  (/.well-known/oauth-authorization-server and /.well-known/openid-configuration 404 on every\n  Markable host probed 2026-08-13); the client_id/client_secret exchange is a vendor-specific\n  endpoint, not RFC 6749 client_credentials.\n- There is no scope surface documented, so scopes/ is intentionally absent. The docs state\n  \"scopes are a concern of tokens and not clients\".\n- The consumer creator-monetization product at app-prod.markable.ai is a separate, unrelated\n  surface with no documented developer authentication.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/markable/refs/heads/main/authentication/markable-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Creator Economy
- Affiliate Marketing
- Social Commerce
- Influencer Marketing
- Content Monetization
- Social Media
- Visual Search
- Computer Vision
- Product Discovery
- Image Recognition
- Video Search
---
