---
anonymous_access: false
api_key_in: []
auth_types: []
description: OAuth authentication is required to keep saved answers and generated PDFs private.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: PaperPorter Authentication
name_suffix: Authentication
oauth_flows: []
overview: PaperPorter declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: PaperPorter
provider_slug: paperporter-com
scheme_count: 1
schemes:
- evidence: Sign in once through OAuth to keep saved answers and generated PDFs private.
  how_to_obtain: Sign in through the browser when prompted by the client (Claude Code or ChatGPT) and approve access.
  name: OAuth
  type: oauth2
slug: paperporter-com-authentication
source_filename: paperporter-com-authentication.yml
source_heading: Authentication Profile
source_url: https://paperporter.com/docs/claude
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://paperporter.com/docs/claude\nsources:\n- https://paperporter.com/docs/claude\n- https://paperporter.com/docs/chatgpt\ndescription: OAuth authentication is required to keep saved answers and generated PDFs private.\nschemes:\n- type: oauth2\n  name: OAuth\n  evidence: Sign in once through OAuth to keep saved answers and generated PDFs private.\n  how_to_obtain: Sign in through the browser when prompted by the client (Claude Code or ChatGPT) and approve access.\ndocs: https://paperporter.com/docs/claude\n"
source_yaml_url: https://artifacts.apis.io/paperporter-com/authentication/paperporter-com-authentication.yml
summary_line: 1 scheme
tags:
- Permits
- PDF Tools
- AI Assistant
- Building Permits
- Food truck permits
- MCP
---
