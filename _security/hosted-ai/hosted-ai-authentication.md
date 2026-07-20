---
api_key_in:
- header
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Hosted Ai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Hosted·ai secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Hosted·ai
provider_slug: hosted-ai
scheme_count: 2
schemes:
- description: Primary authentication for the Admin Panel and User Panel REST API. Users create a named API token in the User Panel (Account Settings > Security > Manage API Tokens) and pass it as an HTTP bearer token. Base URL is per deployment at https://USER_PANEL_URL/api. The full token value is displayed once at creation, then obfuscated. Tokens carry a configurable expiry (short- or long-term) and an optional IP allowlist (single IP or range).
  header: 'Authorization: Bearer [example key]'
  ip_allowlist: optional single IP or IP range per token
  name: bearerToken
  scheme: bearer
  sources:
  - https://docs.hosted.ai/user-panel/faqs/api-faqs
  token_creation: User Panel > Account Settings > Security > Manage API Tokens
  token_expiry: configurable per token
  type: http
- description: OAuth authorize flow recommended for new marketplace integrations (linking marketplace pods/tokens). Plaintext marketplace token linking is marked legacy as of Admin Panel 2.4.1 and OAuth is the recommended path forward.
  flows:
  - flow: authorizationCode
  name: marketplaceOAuth
  sources:
  - https://docs.hosted.ai/releases-notes/release-api-changelogs/admin-panel/241-api-changelogs
  type: oauth2
slug: hosted-ai-authentication
source_filename: hosted-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.hosted.ai/user-panel/faqs/api-faqs\ndocs:\n- https://docs.hosted.ai/user-panel/account-settings-22t5_c/security/manage-api-tokens\n- https://docs.hosted.ai/user-panel/faqs/api-faqs\nsummary:\n  types:\n  - http\n  - oauth2\n  http_schemes:\n  - bearer\n  oauth2_flows:\n  - authorizationCode\n  api_key_in:\n  - header\nschemes:\n- name: bearerToken\n  type: http\n  scheme: bearer\n  description: >-\n    Primary authentication for the Admin Panel and User Panel REST API. Users\n    create a named API token in the User Panel (Account Settings > Security >\n    Manage API Tokens) and pass it as an HTTP bearer token. Base URL is per\n    deployment at https://USER_PANEL_URL/api. The full token value is displayed\n    once at creation, then obfuscated. Tokens carry a configurable expiry\n    (short- or long-term) and an optional IP allowlist (single IP or range).\n  header: 'Authorization: Bearer [example key]'\n  token_creation:\
  \ User Panel > Account Settings > Security > Manage API Tokens\n  token_expiry: configurable per token\n  ip_allowlist: optional single IP or IP range per token\n  sources:\n  - https://docs.hosted.ai/user-panel/faqs/api-faqs\n- name: marketplaceOAuth\n  type: oauth2\n  description: >-\n    OAuth authorize flow recommended for new marketplace integrations (linking\n    marketplace pods/tokens). Plaintext marketplace token linking is marked\n    legacy as of Admin Panel 2.4.1 and OAuth is the recommended path forward.\n  flows:\n  - flow: authorizationCode\n  sources:\n  - https://docs.hosted.ai/releases-notes/release-api-changelogs/admin-panel/241-api-changelogs\nnotes:\n- >-\n  A 401 Unauthorized is documented as an authentication failure; the docs\n  recommend creating a new unrestricted token when troubleshooting 401s.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hosted-ai/refs/heads/main/authentication/hosted-ai-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Ai
- GPU
- GPUaaS
- Cloud Infrastructure
- Neocloud
- Machine Learning
- AI Infrastructure
- Multi-Tenancy
- Service Providers
---
