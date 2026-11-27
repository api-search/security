---
anonymous_access: false
api_key_in: []
api_specs:
- filename: magicscreenshots-com-functions-api-openapi.yml
  format: yaml
  label: MagicScreenshots Functions API
  slug: magicscreenshots-com-functions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/magicscreenshots-com/openapi/magicscreenshots-com-functions-api-openapi.yml
- filename: magicscreenshots-com-mcp-api-openapi.yml
  format: yaml
  label: MagicScreenshots MCP API
  slug: magicscreenshots-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/magicscreenshots-com/openapi/magicscreenshots-com-mcp-api-openapi.yml
auth_types: []
description: Authentication schemes for MagicScreenshots MCP API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: MagicScreenshots Authentication
name_suffix: Authentication
oauth_flows: []
overview: MagicScreenshots declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: MagicScreenshots
provider_slug: magicscreenshots-com
scheme_count: 1
schemes:
- evidence: 'Use Streamable HTTP with URL https://www.magicscreenshots.com/api/mcp and header Authorization: Bearer $MAGICSCREENSHOTS_API_KEY .'
  header: Authorization
  how_to_obtain: create_api_key or Settings > API
  location: header
  name: MagicScreenshots API Key
  type: http-bearer
slug: magicscreenshots-com-authentication
source_filename: magicscreenshots-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.magicscreenshots.com/mcp/docs
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.magicscreenshots.com/mcp/docs\nsources:\n- https://www.magicscreenshots.com/mcp/docs\ndescription: Authentication schemes for MagicScreenshots MCP API\nschemes:\n- type: http-bearer\n  name: MagicScreenshots API Key\n  evidence: 'Use Streamable HTTP with URL https://www.magicscreenshots.com/api/mcp and header Authorization: Bearer $MAGICSCREENSHOTS_API_KEY\n    .'\n  location: header\n  header: Authorization\n  how_to_obtain: create_api_key or Settings > API\ndocs: https://www.magicscreenshots.com/mcp/docs\n"
source_yaml_url: https://artifacts.apis.io/magicscreenshots-com/authentication/magicscreenshots-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- App Store
- Screenshots
- Localization
- Artificial Intelligence
---
