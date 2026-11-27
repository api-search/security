---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: ClimbPast Authentication
name_suffix: Authentication
oauth_flows: []
overview: ClimbPast declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ClimbPast
provider_slug: climbpast-com
scheme_count: 1
schemes:
- applies_to: https://climbpast.com/api/mcp
  description: 'Authentication is a single Bearer token: your cp_ key from your dashboard.'
  format: 'Authorization: Bearer cp_YOUR_KEY'
  header: Authorization
  in: header
  issuance: Create one from the dashboard, or find existing keys under Settings > API Keys.
  key_prefixes_documented:
  - cp_
  - cp_live_ (example token shown in the claude.ai connector instructions)
  name: cp_key
  revocation: Revoke a cp_ key from your dashboard and it stops working immediately.
  scheme: bearer
  type: http
slug: climbpast-com-authentication
source_filename: climbpast-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: ClimbPast authentication\ngenerated: '2026-11-04'\nmethod: searched\nsource: https://climbpast.com/docs/mcp\ndocs: https://climbpast.com/docs/mcp\nnote: No OpenAPI is published; the auth profile is read from the MCP docs and the llms-full.txt index. Auth endpoints were not called.\nschemes:\n- name: cp_key\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer cp_YOUR_KEY'\n  applies_to: https://climbpast.com/api/mcp\n  description: \"Authentication is a single Bearer token: your cp_ key from your dashboard.\"\n  issuance: Create one from the dashboard, or find existing keys under Settings > API Keys.\n  revocation: Revoke a cp_ key from your dashboard and it stops working immediately.\n  key_prefixes_documented: ['cp_', 'cp_live_ (example token shown in the claude.ai connector instructions)']\nupstream_oauth:\n  provider: Google OAuth 2.0 (verified Google app)\n  description: Users connect Google through ClimbPast's verified\
  \ OAuth app; tokens are stored encrypted and never given to the agent.\n  default_scopes_documented: [analytics.readonly, webmasters.readonly]\n  scopes_source: https://climbpast.com/llms-full.txt\n  write_access: Write access is a separate opt-in you enable in Settings, which triggers its own Google consent screen.\n"
source_yaml_url: https://artifacts.apis.io/climbpast-com/authentication/climbpast-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- MCP
- Google Analytics
- Search Console
- Google Tag Manager
- Analytics
- SEO
- AI Agents
---
