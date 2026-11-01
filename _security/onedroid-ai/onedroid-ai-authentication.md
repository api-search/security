---
anonymous_access: false
api_key_in: []
api_specs:
- filename: onedroid-ai-api-openapi.json
  format: json
  label: Trilix MCP Assistant Api API
  slug: trilix-mcp-assistant-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onedroid-ai/openapi/_original/onedroid-ai-api-openapi.json
auth_types: []
description: OneDroid services use bearer tokens passed in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Onedroid Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: onedroid-ai declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: onedroid-ai
provider_slug: onedroid-ai
scheme_count: 1
schemes:
- evidence: 'One command, one header. Then claude mcp list should show synapse … ✓ Connected . claude mcp add --transport http synapse \ https://synapse.onedroid.ai/agent/mcp \ --header "Authorization: Bearer <token>"'
  header: Authorization
  how_to_obtain: In the hub, go to Manage → API Tokens → Create token. The token is shown once and must be copied.
  location: header
  name: Bearer token
  type: http-bearer
slug: onedroid-ai-authentication
source_filename: onedroid-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://onedroid.ai/quickstart
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://onedroid.ai/quickstart\nsources:\n- https://onedroid.ai/quickstart\ndescription: OneDroid services use bearer tokens passed in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'One command, one header. Then claude mcp list should show synapse … ✓ Connected . claude mcp add --transport http synapse \\ https://synapse.onedroid.ai/agent/mcp\n    \\ --header \"Authorization: Bearer <token>\"'\n  location: header\n  header: Authorization\n  how_to_obtain: In the hub, go to Manage → API Tokens → Create token. The token is shown once and must be copied.\nnote: No OAuth2, API key query, or other authentication methods are documented on the page.\ndocs: https://onedroid.ai/quickstart\n"
source_yaml_url: https://artifacts.apis.io/onedroid-ai/authentication/onedroid-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI
- Testing
- Automation
- End-to-End
---
