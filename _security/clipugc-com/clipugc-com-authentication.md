---
anonymous_access: false
api_key_in: []
api_specs:
- filename: clipugc-com-characters-api-openapi.yml
  format: yaml
  label: ClipUGC Characters API
  slug: clipugc-com-characters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipugc-com/openapi/clipugc-com-characters-api-openapi.yml
- filename: clipugc-com-clips-api-openapi.yml
  format: yaml
  label: ClipUGC Clips API
  slug: clipugc-com-clips-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipugc-com/openapi/clipugc-com-clips-api-openapi.yml
- filename: clipugc-com-credits-api-openapi.yml
  format: yaml
  label: ClipUGC Credits API
  slug: clipugc-com-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipugc-com/openapi/clipugc-com-credits-api-openapi.yml
- filename: clipugc-com-finished-videos-api-openapi.yml
  format: yaml
  label: ClipUGC Finished videos API
  slug: clipugc-com-finished-videos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipugc-com/openapi/clipugc-com-finished-videos-api-openapi.yml
- filename: clipugc-com-hooks-api-openapi.yml
  format: yaml
  label: ClipUGC Hooks API
  slug: clipugc-com-hooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipugc-com/openapi/clipugc-com-hooks-api-openapi.yml
- filename: clipugc-com-looks-api-openapi.yml
  format: yaml
  label: ClipUGC Looks API
  slug: clipugc-com-looks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipugc-com/openapi/clipugc-com-looks-api-openapi.yml
- filename: clipugc-com-uploads-api-openapi.yml
  format: yaml
  label: ClipUGC Uploads API
  slug: clipugc-com-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipugc-com/openapi/clipugc-com-uploads-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: ClipUGC Authentication
name_suffix: Authentication
oauth_flows: []
overview: ClipUGC secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ClipUGC
provider_slug: clipugc-com
scheme_count: 1
schemes:
- description: Your API key from Dashboard, API Keys. Needs the Professional or Business plan.
  guidance: A key acts as your account and spends its credits, so keep it on your server and never ship it in an app.
  header: 'Authorization: Bearer YOUR_API_KEY'
  key_issuance: Dashboard > API Keys (https://clipugc.com/dashboard/api-keys); key shown once; several keys allowed, each revocable.
  name: http
  plan_requirement: Keys work while your account is on Professional or Business, including a trial. When the subscription ends, at the end of the paid period, the keys pause.
  scheme: bearer
  sources:
  - openapi/clipugc-com-openapi.yml
  type: http
slug: clipugc-com-authentication
source_filename: clipugc-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://clipugc.com/docs/api\nsummary:\n  types:\n  - http\nschemes:\n- name: http\n  type: http\n  scheme: bearer\n  description: Your API key from Dashboard, API Keys. Needs the Professional or Business\n    plan.\n  sources:\n  - openapi/clipugc-com-openapi.yml\n  header: 'Authorization: Bearer YOUR_API_KEY'\n  key_issuance: Dashboard > API Keys (https://clipugc.com/dashboard/api-keys); key\n    shown once; several keys allowed, each revocable.\n  plan_requirement: Keys work while your account is on Professional or Business, including\n    a trial. When the subscription ends, at the end of the paid period, the keys pause.\n  guidance: A key acts as your account and spends its credits, so keep it on your\n    server and never ship it in an app.\ndocs: https://clipugc.com/docs/api\nother_surfaces:\n- surface: Hosted MCP server https://clipugc.com/mcp\n  auth: OAuth 2.1 with PKCE, sign in with your ClipUGC account\n  source:\
  \ https://clipugc.com/llms-full.txt\n- surface: clipugc CLI / local MCP\n  auth: API key via `clipugc auth login`, stored in ~/.config/clipugc/config.json\n  source: https://github.com/clipugc/ClipUGC-CLI\n"
source_yaml_url: https://artifacts.apis.io/clipugc-com/authentication/clipugc-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- AI Video Generation
- UGC
- AI Influencers
- Mobile App Marketing
- Video
- MCP
- CLI
---
