---
anonymous_access: false
api_key_in: []
api_specs:
- filename: kaptionai-com-mcp-api-openapi.yml
  format: yaml
  label: Kaption AI MCP API
  slug: kaptionai-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaptionai-com/openapi/kaptionai-com-mcp-api-openapi.yml
auth_types: []
description: Authentication OAuth 2.1 with PKCE (S256) and dynamic client registration. There is one scope, kaption:access.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Kaption AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kaption AI declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Kaption AI
provider_slug: kaptionai-com
scheme_count: 2
schemes:
- evidence: Authentication OAuth 2.1 with PKCE (S256) and dynamic client registration. There is one scope, kaption:access.
  flows:
  - authorization_code
  how_to_obtain: Users sign in with their phone number and a code sent to them on WhatsApp, then choose how long the connection lasts.
  name: OAuth 2.1
  scopes:
  - kaption:access
  type: oauth2
- evidence: bearer_methods_supported:["header"]
  header: Authorization
  location: header
  name: Bearer Token
  type: http-bearer
slug: kaptionai-com-authentication
source_filename: kaptionai-com-authentication.yml
source_heading: Authentication Profile
source_url: https://mcp.kaptionai.com/.well-known/oauth-protected-resource/mcp
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mcp.kaptionai.com/.well-known/oauth-protected-resource/mcp\nsources:\n- https://mcp.kaptionai.com/.well-known/oauth-protected-resource/mcp\n- https://kaptionai.com/developers/\n- https://kaptionai.com/mcp/\ndescription: Authentication OAuth 2.1 with PKCE (S256) and dynamic client registration. There is one scope, kaption:access.\nschemes:\n- type: oauth2\n  name: OAuth 2.1\n  evidence: Authentication OAuth 2.1 with PKCE (S256) and dynamic client registration. There is one scope, kaption:access.\n  flows:\n  - authorization_code\n  scopes:\n  - kaption:access\n  how_to_obtain: Users sign in with their phone number and a code sent to them on WhatsApp, then choose how long the connection lasts.\n- type: http-bearer\n  name: Bearer Token\n  evidence: bearer_methods_supported:[\"header\"]\n  location: header\n  header: Authorization\ndocs: https://mcp.kaptionai.com/.well-known/oauth-protected-resource/mcp\n"
source_yaml_url: https://artifacts.apis.io/kaptionai-com/authentication/kaptionai-com-authentication.yml
summary_line: 2 schemes
tags:
- AI Assistant
- Transcription
- Call Recording
- Translation
- Scheduling
- Backups
---
