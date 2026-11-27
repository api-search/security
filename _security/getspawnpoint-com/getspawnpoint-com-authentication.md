---
anonymous_access: false
api_key_in: []
api_specs:
- filename: getspawnpoint-com-openapi-generated.yml
  format: yaml
  label: Spawnpoint API
  slug: getspawnpoint-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getspawnpoint-com/openapi/_ae-authored/getspawnpoint-com-openapi-generated.yml
auth_types: []
description: Authentication methods published for Spawnpoint
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Spawnpoint Authentication
name_suffix: Authentication
oauth_flows: []
overview: Spawnpoint declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Spawnpoint
provider_slug: getspawnpoint-com
scheme_count: 1
schemes:
- evidence: 'Send it as the bearer token on the MCP endpoint: Authorization: Bearer spk_live_your_token'
  header: Authorization
  how_to_obtain: Create a token in the console under API tokens panel; copy the spk_live_… value shown once.
  location: header
  name: API token
  type: http-bearer
slug: getspawnpoint-com-authentication
source_filename: getspawnpoint-com-authentication.yml
source_heading: Authentication Profile
source_url: https://getspawnpoint.com/api-tokens.html
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://getspawnpoint.com/api-tokens.html\nsources:\n- https://getspawnpoint.com/api-tokens.html\n- https://getspawnpoint.com/getting-started.html\ndescription: Authentication methods published for Spawnpoint\nschemes:\n- type: http-bearer\n  name: API token\n  evidence: 'Send it as the bearer token on the MCP endpoint: Authorization: Bearer spk_live_your_token'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a token in the console under API tokens panel; copy the spk_live_… value shown once.\nnote: OAuth flows are mentioned but no token or authorize URLs, scopes, or flow details are provided on the pages.\ndocs: https://getspawnpoint.com/api-tokens.html\n"
source_yaml_url: https://artifacts.apis.io/getspawnpoint-com/authentication/getspawnpoint-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Platform
- Developer Tools
- Software-as-a-Service
- Automation
---
