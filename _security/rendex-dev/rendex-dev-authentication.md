---
anonymous_access: false
api_key_in: []
api_specs:
- filename: rendex-dev-account-api-openapi.yml
  format: yaml
  label: rendex-dev Account API
  slug: rendex-dev-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendex-dev/openapi/rendex-dev-account-api-openapi.yml
- filename: rendex-dev-batch-api-openapi.yml
  format: yaml
  label: rendex-dev Batch API
  slug: rendex-dev-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendex-dev/openapi/rendex-dev-batch-api-openapi.yml
- filename: rendex-dev-health-api-openapi.yml
  format: yaml
  label: rendex-dev Health API
  slug: rendex-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendex-dev/openapi/rendex-dev-health-api-openapi.yml
- filename: rendex-dev-jobs-api-openapi.yml
  format: yaml
  label: rendex-dev Jobs API
  slug: rendex-dev-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendex-dev/openapi/rendex-dev-jobs-api-openapi.yml
- filename: rendex-dev-screenshot-api-openapi.yml
  format: yaml
  label: rendex-dev Screenshot API
  slug: rendex-dev-screenshot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendex-dev/openapi/rendex-dev-screenshot-api-openapi.yml
- filename: rendex-dev-watch-api-openapi.yml
  format: yaml
  label: rendex-dev Watch API
  slug: rendex-dev-watch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendex-dev/openapi/rendex-dev-watch-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Rendex Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: rendex-dev declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: rendex-dev
provider_slug: rendex-dev
scheme_count: 3
schemes:
- description: Bearer token authentication using API key prefixed with rdx_
  name: Authorization
  scheme: bearer
  type: http
- description: API key passed in X-API-Key header
  in: header
  name: x-api-key
  type: apiKey
- description: API key passed as query parameter 'key'
  in: query
  name: key
  type: apiKey
slug: rendex-dev-authentication
source_filename: rendex-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://rendex.dev/docs/authentication\nschemes:\n  - type: http\n    scheme: bearer\n    name: Authorization\n    description: \"Bearer token authentication using API key prefixed with rdx_\"\n  - type: apiKey\n    name: \"x-api-key\"\n    in: header\n    description: \"API key passed in X-API-Key header\"\n  - type: apiKey\n    name: \"key\"\n    in: query\n    description: \"API key passed as query parameter 'key'\"\n"
source_yaml_url: https://artifacts.apis.io/rendex-dev/authentication/rendex-dev-authentication.yml
summary_line: 3 schemes
tags:
- Rendering
- Screenshot
- PDF
- API
- Automation
---
