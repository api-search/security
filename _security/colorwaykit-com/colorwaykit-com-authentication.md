---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: ColorwayKit Authentication
name_suffix: Authentication
oauth_flows: []
overview: ColorwayKit declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ColorwayKit
provider_slug: colorwaykit-com
scheme_count: 1
schemes:
- applies_to: https://www.colorwaykit.com/api/mcp
  description: 'Agent token (prefix ck_) generated on the MCP page after signing in to a free account; sent as "Authorization: Bearer ck_..." by the MCP client.'
  format: Bearer ck_YOUR_TOKEN
  header: Authorization
  name: agentToken
  scheme: bearer
  type: http
slug: colorwaykit-com-authentication
source_filename: colorwaykit-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://www.colorwaykit.com/mcp\ndocs: https://www.colorwaykit.com/mcp\nnote: No OpenAPI is published; the only programmatic surface is the remote MCP server. A probe of https://www.colorwaykit.com/api/mcp without credentials returned 401 (preflight 2026-11-04).\nschemes:\n- name: agentToken\n  type: http\n  scheme: bearer\n  header: Authorization\n  format: 'Bearer ck_YOUR_TOKEN'\n  description: 'Agent token (prefix ck_) generated on the MCP page after signing in to a free account; sent as \"Authorization: Bearer ck_...\" by the MCP client.'\n  applies_to: https://www.colorwaykit.com/api/mcp\n"
source_yaml_url: https://artifacts.apis.io/colorwaykit-com/authentication/colorwaykit-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Color
- Design Tokens
- Accessibility
- Theming
- MCP
- AI Agents
- Developer Tools
---
