---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ogstamp-com-auto-api-openapi.yml
  format: yaml
  label: ogstamp-com Auto API
  slug: ogstamp-com-auto-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ogstamp-com/openapi/ogstamp-com-auto-api-openapi.yml
- filename: ogstamp-com-credits-api-openapi.yml
  format: yaml
  label: ogstamp-com Credits API
  slug: ogstamp-com-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ogstamp-com/openapi/ogstamp-com-credits-api-openapi.yml
- filename: ogstamp-com-mcp-api-openapi.yml
  format: yaml
  label: ogstamp-com MCP API
  slug: ogstamp-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ogstamp-com/openapi/ogstamp-com-mcp-api-openapi.yml
- filename: ogstamp-com-og-api-openapi.yml
  format: yaml
  label: ogstamp-com Og API
  slug: ogstamp-com-og-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ogstamp-com/openapi/ogstamp-com-og-api-openapi.yml
- filename: ogstamp-com-packs-api-openapi.yml
  format: yaml
  label: ogstamp-com Packs API
  slug: ogstamp-com-packs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ogstamp-com/openapi/ogstamp-com-packs-api-openapi.yml
- filename: ogstamp-com-peek-api-openapi.yml
  format: yaml
  label: ogstamp-com Peek API
  slug: ogstamp-com-peek-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ogstamp-com/openapi/ogstamp-com-peek-api-openapi.yml
- filename: ogstamp-com-recover-api-openapi.yml
  format: yaml
  label: ogstamp-com Recover API
  slug: ogstamp-com-recover-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ogstamp-com/openapi/ogstamp-com-recover-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Ogstamp Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: ogstamp-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ogstamp-com
provider_slug: ogstamp-com
scheme_count: 2
schemes:
- description: API key prefixed with ogs_, sent in Authorization header
  scheme: bearer
  type: http
- description: Alternative header for API key
  in: header
  name: X-Api-Key
  type: apiKey
slug: ogstamp-com-authentication
source_filename: ogstamp-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://ogstamp.com/docs/\nschemes:\n  - type: http\n    scheme: bearer\n    description: API key prefixed with ogs_, sent in Authorization header\n  - type: apiKey\n    name: X-Api-Key\n    in: header\n    description: Alternative header for API key\n"
source_yaml_url: https://artifacts.apis.io/ogstamp-com/authentication/ogstamp-com-authentication.yml
summary_line: 2 schemes
tags:
- Open Graph
- Image Generation
- API
- Pay-as-you-go
- Social Media
---
