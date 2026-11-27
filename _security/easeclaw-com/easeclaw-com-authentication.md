---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication for EaseClaw MCP uses a Bearer token sent in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: EaseClaw Authentication
name_suffix: Authentication
oauth_flows: []
overview: EaseClaw declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: EaseClaw
provider_slug: easeclaw-com
scheme_count: 1
schemes:
- evidence: '—header "Authorization: Bearer ec_live_YOUR_KEY"'
  header: Authorization
  location: header
  name: Bearer
  type: http-bearer
slug: easeclaw-com-authentication
source_filename: easeclaw-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.easeclaw.com/mcp
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.easeclaw.com/mcp\nsources:\n- https://www.easeclaw.com/mcp\ndescription: Authentication for EaseClaw MCP uses a Bearer token sent in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: '—header \"Authorization: Bearer ec_live_YOUR_KEY\"'\n  location: header\n  header: Authorization\nnote: OAuth flows are mentioned for Claude.ai and ChatGPT connections, but no token or authorize URLs, scopes, or flow details are provided on\n  the page.\ndocs: https://www.easeclaw.com/mcp\n"
source_yaml_url: https://artifacts.apis.io/easeclaw-com/authentication/easeclaw-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Sales
- LinkedIn
- Outreach
- Automation
---
