---
anonymous_access: false
api_key_in: []
auth_types: []
description: Kleo MCP uses OAuth 2.1 for authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Kleo AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kleo AI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Kleo AI
provider_slug: kleooai-com
scheme_count: 1
schemes:
- evidence: Auth OAuth 2.1. During authorization the client opens Kleo’s own page; you click Start free and you are back in the client with 5 credits on the account.
  header: Authorization
  how_to_obtain: Client opens Kleo’s sign‑in page, clicks “Start free”, and receives an OAuth token.
  location: header
  name: OAuth 2.1
  type: oauth2
slug: kleooai-com-authentication
source_filename: kleooai-com-authentication.yml
source_heading: Authentication Profile
source_url: https://kleooai.com/video-generation-mcp/
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://kleooai.com/video-generation-mcp/\nsources:\n- https://kleooai.com/video-generation-mcp/\n- https://kleooai.com/integrations/claude/\n- https://kleooai.com/integrations/chatgpt/\n- https://kleooai.com/guides/free/\ndescription: Kleo MCP uses OAuth 2.1 for authentication.\nschemes:\n- type: oauth2\n  name: OAuth 2.1\n  evidence: Auth OAuth 2.1. During authorization the client opens Kleo’s own page; you click Start free and you are back in the client with 5\n    credits on the account.\n  location: header\n  header: Authorization\n  how_to_obtain: Client opens Kleo’s sign‑in page, clicks “Start free”, and receives an OAuth token.\ndocs: https://kleooai.com/video-generation-mcp/\n"
source_yaml_url: https://artifacts.apis.io/kleooai-com/authentication/kleooai-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Video
- Image
- Voice
- Creative
---
