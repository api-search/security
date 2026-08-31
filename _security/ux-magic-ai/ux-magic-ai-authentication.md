---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Ux Magic Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: UX Magic AI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: UX Magic AI
provider_slug: ux-magic-ai
scheme_count: 1
schemes:
- applies_to: https://api.uxmagic.ai/api/mcp (MCP server, Streamable HTTP)
  in: header
  key_management: https://uxmagic.ai/manage-account?value=api-keys
  key_prefix: uxm_
  name: X-API-Key
  parameter: X-API-Key
  scope_note: Per provider docs, a key with no scopes has full access.
  scopes:
  - description: Read access to designs, projects, frames, themes, and documents.
    name: designs:read
  - description: Create and edit projects, frames, and designs; export to Figma.
    name: designs:write
  - description: Run AI design generation and agent operations.
    name: agent:run
  sources:
  - https://uxmagic.ai/docs/connect-mcp
  - https://www.npmjs.com/package/uxmagic-mcp
  type: apiKey
slug: ux-magic-ai-authentication
source_filename: ux-magic-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://uxmagic.ai/docs/connect-mcp\ndocs: https://uxmagic.ai/docs/connect-mcp\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: X-API-Key\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  key_prefix: uxm_\n  key_management: https://uxmagic.ai/manage-account?value=api-keys\n  applies_to: https://api.uxmagic.ai/api/mcp (MCP server, Streamable HTTP)\n  scopes:\n  - name: designs:read\n    description: Read access to designs, projects, frames, themes, and documents.\n  - name: designs:write\n    description: Create and edit projects, frames, and designs; export to Figma.\n  - name: agent:run\n    description: Run AI design generation and agent operations.\n  scope_note: Per provider docs, a key with no scopes has full access.\n  sources:\n  - https://uxmagic.ai/docs/connect-mcp\n  - https://www.npmjs.com/package/uxmagic-mcp\nenterprise:\n  sso_saml: true\n  source: https://uxmagic.ai/pricing\
  \ (Enterprise plan lists SSO / SAML authentication)\nnotes: >-\n  UXMagic publishes no OpenAPI; its machine surface is the MCP server at\n  https://api.uxmagic.ai/api/mcp authenticated with per-key-scoped API keys\n  (uxm_ prefix) sent in the X-API-Key header. Keys are generated in the UXMagic\n  editor (Connect MCP -> Generate your API Key) or Settings -> API Keys.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ux-magic-ai/refs/heads/main/authentication/ux-magic-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Design
- ArtificialIntelligence
- UIDesign
- UXDesign
- Figma
- DesignToCode
- MCP
- Wireframes
---
