---
anonymous_access: false
api_key_in: []
api_specs:
- filename: brain-tube-com-api-openapi.json
  format: json
  label: BrainTube REST API API
  slug: braintube-rest-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brain-tube-com/openapi/_original/brain-tube-com-api-openapi.json
auth_types: []
description: Authentication methods for BrainTube as documented
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: BrainTube Authentication
name_suffix: Authentication
oauth_flows: []
overview: BrainTube declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: BrainTube
provider_slug: brain-tube-com
scheme_count: 2
schemes:
- evidence: 'Include it in requests: Authorization: Bearer bt_sk_your_api_key_here'
  header: Authorization
  how_to_obtain: Generate an API key from Settings → API Keys.
  location: header
  name: Bearer
  type: http-bearer
- evidence: ChatGPT adds remote MCP servers under Settings › Plugins › Add custom MCP server, and BrainTube works there with OAuth.
  how_to_obtain: Sign in through the OAuth flow in the client UI (e.g., ChatGPT or Claude).
  name: OAuth
  type: oauth2
slug: brain-tube-com-authentication
source_filename: brain-tube-com-authentication.yml
source_heading: Authentication Profile
source_url: https://brain-tube.com/guide/give-your-ai-memory-mcp
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://brain-tube.com/guide/give-your-ai-memory-mcp\nsources:\n- https://brain-tube.com/guide/give-your-ai-memory-mcp\n- https://brain-tube.com/support/category/getting-started\n- https://brain-tube.com/support/article/rest-api-quickstart\ndescription: Authentication methods for BrainTube as documented\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Include it in requests: Authorization: Bearer bt_sk_your_api_key_here'\n  location: header\n  header: Authorization\n  how_to_obtain: Generate an API key from Settings → API Keys.\n- type: oauth2\n  name: OAuth\n  evidence: ChatGPT adds remote MCP servers under Settings › Plugins › Add custom MCP server, and BrainTube works there with OAuth.\n  how_to_obtain: Sign in through the OAuth flow in the client UI (e.g., ChatGPT or Claude).\ndocs: https://brain-tube.com/guide/give-your-ai-memory-mcp\n"
source_yaml_url: https://artifacts.apis.io/brain-tube-com/authentication/brain-tube-com-authentication.yml
summary_line: 2 schemes
tags:
- AI Integration
- MCP
---
