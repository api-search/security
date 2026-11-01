---
anonymous_access: false
api_key_in: []
api_specs:
- filename: corsproxy-dev-health-api-openapi.yml
  format: yaml
  label: corsproxy-dev Health API
  slug: corsproxy-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corsproxy-dev/openapi/corsproxy-dev-health-api-openapi.yml
- filename: corsproxy-dev-mcp-api-openapi.yml
  format: yaml
  label: corsproxy-dev MCP API
  slug: corsproxy-dev-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corsproxy-dev/openapi/corsproxy-dev-mcp-api-openapi.yml
- filename: corsproxy-dev-proxy-api-openapi.yml
  format: yaml
  label: corsproxy-dev Proxy API
  slug: corsproxy-dev-proxy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corsproxy-dev/openapi/corsproxy-dev-proxy-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Corsproxy Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: corsproxy-dev declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: corsproxy-dev
provider_slug: corsproxy-dev
scheme_count: 1
schemes:
- description: For server-side proxy calls. Browser callers should use the `?key=` query param instead.
  in: header
  name: X-API-Key
  type: apiKey
slug: corsproxy-dev-authentication
source_filename: corsproxy-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: https://corsproxy.dev/openapi.yaml\nschemes:\n  - type: apiKey\n    name: X-API-Key\n    in: header\n    description: For server-side proxy calls. Browser callers should use the `?key=` query param instead.\n"
source_yaml_url: https://artifacts.apis.io/corsproxy-dev/authentication/corsproxy-dev-authentication.yml
summary_line: 1 scheme
tags:
- Company
- CORS
- Proxy
- API
- Developer Tools
- Open Source
---
