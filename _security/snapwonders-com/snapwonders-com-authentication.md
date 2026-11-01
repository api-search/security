---
anonymous_access: false
api_key_in: []
api_specs:
- filename: snapwonders-com-analyse-api-openapi.yml
  format: yaml
  label: snapwonders-com Analyse API
  slug: snapwonders-com-analyse-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snapwonders-com/openapi/snapwonders-com-analyse-api-openapi.yml
- filename: snapwonders-com-convert-api-openapi.yml
  format: yaml
  label: snapwonders-com Convert API
  slug: snapwonders-com-convert-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snapwonders-com/openapi/snapwonders-com-convert-api-openapi.yml
- filename: snapwonders-com-hide-api-openapi.yml
  format: yaml
  label: snapwonders-com Hide API
  slug: snapwonders-com-hide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snapwonders-com/openapi/snapwonders-com-hide-api-openapi.yml
- filename: snapwonders-com-mcp-api-openapi.yml
  format: yaml
  label: snapwonders-com MCP API
  slug: snapwonders-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snapwonders-com/openapi/snapwonders-com-mcp-api-openapi.yml
- filename: snapwonders-com-media-upload-direct-api-openapi.yml
  format: yaml
  label: snapwonders-com Media Upload - Direct API
  slug: snapwonders-com-media-upload-direct-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snapwonders-com/openapi/snapwonders-com-media-upload-direct-api-openapi.yml
- filename: snapwonders-com-media-upload-tus-resumable-api-openapi.yml
  format: yaml
  label: snapwonders-com Media Upload - TUS Resumable API
  slug: snapwonders-com-media-upload-tus-resumable-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snapwonders-com/openapi/snapwonders-com-media-upload-tus-resumable-api-openapi.yml
- filename: snapwonders-com-reveal-api-openapi.yml
  format: yaml
  label: snapwonders-com Reveal API
  slug: snapwonders-com-reveal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snapwonders-com/openapi/snapwonders-com-reveal-api-openapi.yml
- filename: snapwonders-com-status-api-openapi.yml
  format: yaml
  label: snapwonders-com Status API
  slug: snapwonders-com-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snapwonders-com/openapi/snapwonders-com-status-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Snapwonders Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: snapwonders-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: snapwonders-com
provider_slug: snapwonders-com
scheme_count: 1
schemes:
- description: API key generated on your snapWONDERS account profile page. Required everywhere except GET /api/status, OPTIONS /api/tus and the no-auth MCP methods.
  in: header
  name: X-Api-Key
  type: apiKey
slug: snapwonders-com-authentication
source_filename: snapwonders-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/snapwonders-com-openapi.json\nschemes:\n  - type: apiKey\n    name: X-Api-Key\n    in: header\n    description: API key generated on your snapWONDERS account profile page. Required everywhere except GET /api/status, OPTIONS /api/tus and the no-auth MCP methods.\n"
source_yaml_url: https://artifacts.apis.io/snapwonders-com/authentication/snapwonders-com-authentication.yml
summary_line: 1 scheme
tags:
- Forensics
- Steganography
- MediaConversion
- Privacy
- Open Source
---
