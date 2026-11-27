---
anonymous_access: true
api_key_in: []
api_specs:
- filename: clipkit-dev-openapi-generated.yml
  format: yaml
  label: Clipkit Render API
  slug: clipkit-dev-render-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipkit-dev/openapi/_ae-authored/clipkit-dev-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Clipkit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clipkit declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Clipkit
provider_slug: clipkit-dev
scheme_count: 2
schemes:
- applies_to:
  - createRender
  - getRender
  description: 'Render API requests send "Authorization: Bearer ${CLIPKIT_API_KEY}". Keys belong to a Clipkit team and can be viewed, rotated or revoked under API Keys (https://www.clipkit.dev/keys); the Vercel Marketplace integration provisions CLIPKIT_API_KEY as an encrypted env var.'
  key_format: 'ck_live_… (docs/mcp: a ck_live_… key from Settings → API keys)'
  name: bearer
  scheme: bearer
  type: http
- description: The hosted MCP endpoint https://www.clipkit.dev/mcp "is open — no sign-in, no OAuth, and no API key for free authoring"; CLIPKIT_API_KEY is only required for the paid render_video tool.
  name: none (MCP hosted connector)
  type: none
slug: clipkit-dev-authentication
source_filename: clipkit-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://www.clipkit.dev/docs/vercel\ndocs: https://www.clipkit.dev/docs/vercel\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: 'Render API requests send \"Authorization: Bearer ${CLIPKIT_API_KEY}\".\n    Keys belong to a Clipkit team and can be viewed, rotated or revoked under API\n    Keys (https://www.clipkit.dev/keys); the Vercel Marketplace integration provisions\n    CLIPKIT_API_KEY as an encrypted env var.'\n  key_format: 'ck_live_… (docs/mcp: a ck_live_… key from Settings → API keys)'\n  applies_to:\n  - createRender\n  - getRender\n- name: none (MCP hosted connector)\n  type: none\n  description: The hosted MCP endpoint https://www.clipkit.dev/mcp \"is open — no sign-in,\n    no OAuth, and no API key for free authoring\"; CLIPKIT_API_KEY is only required\n    for the paid render_video tool.\noauth: false\nnote: No OAuth is documented. No test-mode key prefix is documented.\ndocs_also:\n- https://www.clipkit.dev/docs/mcp\n"
source_yaml_url: https://artifacts.apis.io/clipkit-dev/authentication/clipkit-dev-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Video
- Video Rendering
- AI Agents
- MCP
- JSON
- Open Source
- Developer Tools
---
