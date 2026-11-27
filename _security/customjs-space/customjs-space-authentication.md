---
anonymous_access: false
api_key_in: []
api_specs:
- filename: customjs-space-openapi-generated.yml
  format: yaml
  label: CustomJS API
  slug: customjs-space-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/customjs-space/openapi/_ae-authored/customjs-space-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: CustomJS Authentication
name_suffix: Authentication
oauth_flows: []
overview: CustomJS declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: CustomJS
provider_slug: customjs-space
scheme_count: 3
schemes:
- description: 'All requests require the x-api-key header and Content-Type: application/json. Key is obtained from the dashboard at app.customjs.space (API Key > Show).'
  docs: https://www.customjs.space/integration/native-api/documentation/
  header: x-api-key
  in: header
  name: apiKey
  type: apiKey
- description: The API key guide's JS execution example embeds the key in the URL path, https://e.customjs.io/__js1-YOUR_API_KEY, with no x-api-key header.
  docs: https://www.customjs.space/integration/native-api/api-key
  in: path
  name: apiKeyInPath
  type: apiKey
- applies_to: https://mcp.customjs.space/customjs/mcp
  description: The remote MCP server takes the same API key in the x-api-key header.
  docs: https://www.customjs.space/integration/mcp/
  header: x-api-key
  in: header
  name: mcpApiKey
  type: apiKey
slug: customjs-space-authentication
source_filename: customjs-space-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://www.customjs.space/integration/native-api/api-key\ndocs: https://www.customjs.space/integration/native-api/api-key\nname: CustomJS authentication\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  header: x-api-key\n  description: 'All requests require the x-api-key header and Content-Type: application/json. Key is obtained from the dashboard at app.customjs.space (API Key > Show).'\n  docs: https://www.customjs.space/integration/native-api/documentation/\n- name: apiKeyInPath\n  type: apiKey\n  in: path\n  description: The API key guide's JS execution example embeds the key in the URL path, https://e.customjs.io/__js1-YOUR_API_KEY, with no x-api-key header.\n  docs: https://www.customjs.space/integration/native-api/api-key\n- name: mcpApiKey\n  type: apiKey\n  in: header\n  header: x-api-key\n  applies_to: https://mcp.customjs.space/customjs/mcp\n  description: The remote MCP server takes the same API key in\
  \ the x-api-key header.\n  docs: https://www.customjs.space/integration/mcp/\noauth2: false\nnote: No OAuth, scopes or key types (test/live) are documented.\n"
source_yaml_url: https://artifacts.apis.io/customjs-space/authentication/customjs-space-authentication.yml
summary_line: 3 schemes
tags:
- Company
- JavaScript
- Automation
- PDF Generation
- Screenshots
- No-Code
- Make
- n8n
- MCP
---
