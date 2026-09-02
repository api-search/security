---
api_key_in:
- header
api_specs:
- filename: igaming-tools-openapi.json
  format: json
  label: iGamingScraper REST API
  slug: igamingscraper-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/igaming-tools/refs/heads/main/openapi/igaming-tools-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Igaming Tools Authentication
name_suffix: Authentication
oauth_flows: []
overview: iGaming Tools secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: iGaming Tools
provider_slug: igaming-tools
scheme_count: 1
schemes:
- description: DRF-style token. Header value is the literal word "Token", a space, then the hex key — not "Bearer". Create a free account and issue your own key at /account/; the key is shown once, at creation. Free tier included, no card required.
  format: Token <hex>
  in: header
  name: TokenAuth
  parameter: Authorization
  sources:
  - openapi/igaming-tools-openapi.json
  - https://i-gaming.tools/docs/authentication.md
  type: apiKey
slug: igaming-tools-authentication
source_filename: igaming-tools-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: searched\nsource: https://i-gaming.tools/docs/authentication.md\ndocs: https://i-gaming.tools/docs/authentication/\nspec: openapi/igaming-tools-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  self_service_signup: true\n  note: >-\n    One scheme, applied to every operation in the spec. The MCP server at\n    mcp.i-gaming.tools is a SEPARATE surface with no authentication at all — probed\n    anonymously on 2026-08-30 and it returned the full tool list.\nschemes:\n- name: TokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: Token <hex>\n  description: >-\n    DRF-style token. Header value is the literal word \"Token\", a space, then the hex key —\n    not \"Bearer\". Create a free account and issue your own key at /account/; the key is\n    shown once, at creation. Free tier included, no card required.\n  sources:\n  - openapi/igaming-tools-openapi.json\n\
  \  - https://i-gaming.tools/docs/authentication.md\ntoken_lifecycle:\n  expires: false\n  note: Tokens do not expire by default.\n  issuance: Self-service from the browser dashboard at https://i-gaming.tools/account/ after email confirmation.\n  rotation: Multiple keys may be held per account; any of them can be revoked from the same dashboard page.\n  scope: Each token is scoped to one user account; quota lives on the account, not on the key.\n  key_management_channel: browser-only\n  security_property: >-\n    Provider states key management is browser-only by design: \"a leaked key cannot revoke\n    your other keys or mint itself a replacement.\" Source: /docs/authentication.md.\n  display: Key is displayed once at creation and never again.\nauth_errors:\n- status: 401\n  code: unauthorized\n  meaning: Missing or invalid token.\n- status: 402\n  code: quota_exhausted\n  meaning: Authenticated but the monthly free tier or paid balance is depleted.\n- status: 403\n  code: forbidden\n\
  \  meaning: Endpoint is served to a signed-in browser session and no valid session was presented.\n- status: 429\n  code: throttled\n  meaning: Per-user requests-per-minute cap exceeded; honor Retry-After.\nscopes:\n  supported: false\n  note: >-\n    No OAuth2 or scope model is declared in the spec or the docs. Access is all-or-nothing\n    per token; there is no read/write split because the API is entirely read-only (29 GET\n    operations, zero write operations).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/igaming-tools/refs/heads/main/authentication/igaming-tools-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- iGaming
- Online Casino
- Gambling
- slot games
- slot metadata
- gambling regulation
- Industry News
- Job
- market demand
- Analytics
- REST API
- OpenAPI
- MCP Server
- llms-txt
- LLM Tooling
- slot RTP
- paytable data
- search demand
- iGaming jobs
- agent-ready API
- read-only API
---
