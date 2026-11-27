---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: CodePic Authentication
name_suffix: Authentication
oauth_flows: []
overview: CodePic declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: CodePic
provider_slug: codepic-cc
scheme_count: 1
schemes:
- applies_to: https://codepic.cc/api/mcp/mcp
  description: 'API key created by a signed-in user at codepic.cc/settings/api-keys and sent as "Authorization: Bearer cpk_your_api_key_here" to the remote Streamable HTTP MCP endpoint. The GitHub README calls it "a free API key (the `cpk_...` token)".'
  format: Bearer cpk_...
  header: Authorization
  in: header
  key_prefix: cpk_
  name: bearerApiKey
  provisioning: https://codepic.cc/settings/api-keys
  scheme: bearer
  type: http
slug: codepic-cc-authentication
source_filename: codepic-cc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://codepic.cc/tools/mcp\ndocs: https://github.com/abelce/codepic-mcp\nname: CodePic authentication\nschemes:\n- name: bearerApiKey\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Bearer cpk_...'\n  key_prefix: cpk_\n  applies_to: https://codepic.cc/api/mcp/mcp\n  provisioning: https://codepic.cc/settings/api-keys\n  description: 'API key created by a signed-in user at codepic.cc/settings/api-keys and sent as \"Authorization: Bearer cpk_your_api_key_here\" to the remote Streamable HTTP MCP endpoint. The GitHub README calls it \"a free API key (the `cpk_...` token)\".'\nnote: No OAuth, scopes or REST OpenAPI securitySchemes are published; the MCP server is the only documented programmatic surface.\n"
source_yaml_url: https://artifacts.apis.io/codepic-cc/authentication/codepic-cc-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Whiteboard
- Diagramming
- Flowcharts
- MCP
- AI Agents
- Visual Collaboration
---
