---
anonymous_access: false
api_key_in: []
api_specs:
- filename: clipspeed-ai-openapi-generated.yml
  format: yaml
  label: ClipSpeed API
  slug: clipspeed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipspeed-ai/openapi/_ae-authored/clipspeed-ai-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: ClipSpeedAI Authentication
name_suffix: Authentication
oauth_flows: []
overview: ClipSpeedAI declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: ClipSpeedAI
provider_slug: clipspeed-ai
scheme_count: 3
schemes:
- description: Every request to /api/v1 is authenticated with a personal API key. Keys are tied to one account and inherit that account's plan and rate limit.
  header: X-API-Key
  in: header
  key_format: csai_live_...
  name: X-API-Key
  preferred: true
  type: apiKey
- description: 'The same API key may be sent as "Authorization: Bearer csai_live_..." (documented as an alternative to X-API-Key).'
  header: Authorization
  name: Bearer
  scheme: bearer
  type: http
- applies_to: https://api.clipspeed.ai/mcp
  description: The remote MCP endpoint uses OAuth 2.0; it returns 401 with a WWW-Authenticate header pointing at https://api.clipspeed.ai/.well-known/oauth-protected-resource.
  name: MCP OAuth
  source: https://www.clipspeed.ai/llms-full.txt
  type: oauth2
slug: clipspeed-ai-authentication
source_filename: clipspeed-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://www.clipspeed.ai/developers/\ndocs: https://www.clipspeed.ai/developers/\nname: ClipSpeedAI authentication\nschemes:\n- name: X-API-Key\n  type: apiKey\n  in: header\n  header: X-API-Key\n  preferred: true\n  key_format: csai_live_...\n  description: Every request to /api/v1 is authenticated with a personal API key. Keys are tied to one account and inherit that account's plan and rate limit.\n- name: Bearer\n  type: http\n  scheme: bearer\n  header: Authorization\n  description: 'The same API key may be sent as \"Authorization: Bearer csai_live_...\" (documented as an alternative to X-API-Key).'\n- name: MCP OAuth\n  type: oauth2\n  applies_to: https://api.clipspeed.ai/mcp\n  description: The remote MCP endpoint uses OAuth 2.0; it returns 401 with a WWW-Authenticate header pointing at https://api.clipspeed.ai/.well-known/oauth-protected-resource.\n  source: https://www.clipspeed.ai/llms-full.txt\nkey_management:\n \
  \ issuance: Keys are minted at https://www.clipspeed.ai/dashboard/api-key/ and require a paid plan or the $1 trial.\n  storage: Only a SHA-256 hash of the key is stored server-side; the plaintext is shown once at creation.\n  rotation: Rotate or revoke anytime at /dashboard/api-key/.\n  plan_gate: Free / no-subscription accounts get 403 subscription_required with an upgrade_url.\n"
source_yaml_url: https://artifacts.apis.io/clipspeed-ai/authentication/clipspeed-ai-authentication.yml
summary_line: 3 schemes
tags:
- Company
- AI Video
- Video Clipping
- Image Generation
- Generative AI
- Live Streaming
- Social Media
- MCP
---
