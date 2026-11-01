---
anonymous_access: false
api_key_in: []
api_specs:
- filename: imejis-io-analytics-api-openapi.yml
  format: yaml
  label: imejis-io Analytics API
  slug: imejis-io-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imejis-io/openapi/imejis-io-analytics-api-openapi.yml
- filename: imejis-io-designs-api-openapi.yml
  format: yaml
  label: imejis-io Designs API
  slug: imejis-io-designs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imejis-io/openapi/imejis-io-designs-api-openapi.yml
- filename: imejis-io-keys-api-openapi.yml
  format: yaml
  label: imejis-io Keys API
  slug: imejis-io-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imejis-io/openapi/imejis-io-keys-api-openapi.yml
- filename: imejis-io-render-api-openapi.yml
  format: yaml
  label: imejis-io Render API
  slug: imejis-io-render-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imejis-io/openapi/imejis-io-render-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Imejis Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: imejis-io declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: imejis-io
provider_slug: imejis-io
scheme_count: 3
schemes:
- description: Bearer token authentication (JWT)
  scheme: bearer
  scheme_name: bearerAuth
  type: http
- description: Render API key passed in header
  in: header
  key_name: dma-api-key
  scheme_name: renderKeyHeader
  type: apiKey
- description: Render API key passed as query parameter
  in: query
  key_name: dma-api-key
  scheme_name: renderKeyQuery
  type: apiKey
slug: imejis-io-authentication
source_filename: imejis-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/imejis-io-openapi.json\nschemes:\n  - scheme_name: bearerAuth\n    type: http\n    scheme: bearer\n    description: \"Bearer token authentication (JWT)\"\n  - scheme_name: renderKeyHeader\n    type: apiKey\n    in: header\n    key_name: dma-api-key\n    description: \"Render API key passed in header\"\n  - scheme_name: renderKeyQuery\n    type: apiKey\n    in: query\n    key_name: dma-api-key\n    description: \"Render API key passed as query parameter\"\n"
source_yaml_url: https://artifacts.apis.io/imejis-io/authentication/imejis-io-authentication.yml
summary_line: 3 schemes
tags:
- Company
---
