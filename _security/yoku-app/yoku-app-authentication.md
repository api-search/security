---
anonymous_access: false
api_key_in: []
api_specs:
- filename: yoku-app-openapi-generated.yml
  format: yaml
  label: yoku-app API
  slug: yoku-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yoku-app/openapi/_ae-authored/yoku-app-openapi-generated.yml
auth_types: []
description: Authentication methods for Yoku API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Yoku App Authentication
name_suffix: Authentication
oauth_flows: []
overview: yoku-app declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: yoku-app
provider_slug: yoku-app
scheme_count: 1
schemes:
- evidence: 'All requests to the MCP server must include your API key as a Bearer token in the Authorization header: Authorization: Bearer YOUR_API_KEY'
  header: Authorization
  how_to_obtain: Generate an API key in the Yoku dashboard (Settings > API Keys) and use it as the Bearer token.
  location: header
  name: Bearer token
  type: http-bearer
slug: yoku-app-authentication
source_filename: yoku-app-authentication.yml
source_heading: Authentication Profile
source_url: https://www.yoku.app/docs/getting-started/authentication
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.yoku.app/docs/getting-started/authentication\nsources:\n- https://www.yoku.app/docs/getting-started/authentication\n- https://www.yoku.app/docs/mcp/setup\n- https://www.yoku.app/docs/getting-started\n- https://www.yoku.app/docs/getting-started/concepts\ndescription: Authentication methods for Yoku API\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'All requests to the MCP server must include your API key as a Bearer token in the Authorization header: Authorization: Bearer YOUR_API_KEY'\n  location: header\n  header: Authorization\n  how_to_obtain: Generate an API key in the Yoku dashboard (Settings > API Keys) and use it as the Bearer token.\nnote: No OAuth2, apiKey, or other authentication schemes are documented.\ndocs: https://www.yoku.app/docs/getting-started/authentication\n"
source_yaml_url: https://artifacts.apis.io/yoku-app/authentication/yoku-app-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Brands
- Data
- Software-as-a-Service
---
