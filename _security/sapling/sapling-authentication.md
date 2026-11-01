---
anonymous_access: false
api_key_in: []
api_specs:
- filename: sapling-account-api-openapi.yml
  format: yaml
  label: Sapling Account API
  slug: sapling-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sapling/openapi/sapling-account-api-openapi.yml
- filename: sapling-analysis-api-openapi.yml
  format: yaml
  label: Sapling Analysis API
  slug: sapling-analysis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sapling/openapi/sapling-analysis-api-openapi.yml
- filename: sapling-detection-api-openapi.yml
  format: yaml
  label: Sapling Detection API
  slug: sapling-detection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sapling/openapi/sapling-detection-api-openapi.yml
- filename: sapling-files-api-openapi.yml
  format: yaml
  label: Sapling Files API
  slug: sapling-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sapling/openapi/sapling-files-api-openapi.yml
- filename: sapling-generation-api-openapi.yml
  format: yaml
  label: Sapling Generation API
  slug: sapling-generation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sapling/openapi/sapling-generation-api-openapi.yml
- filename: sapling-proofreading-api-openapi.yml
  format: yaml
  label: Sapling Proofreading API
  slug: sapling-proofreading-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sapling/openapi/sapling-proofreading-api-openapi.yml
- filename: sapling-service-api-openapi.yml
  format: yaml
  label: Sapling Service API
  slug: sapling-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sapling/openapi/sapling-service-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Sapling Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sapling declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Sapling
provider_slug: sapling
scheme_count: 2
schemes:
- description: API key as query parameter
  in: query
  name: key
  type: apiKey
- bearerFormat: JWT
  description: API key as Bearer token in Authorization header
  scheme: bearer
  type: http
slug: sapling-authentication
source_filename: sapling-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: searched\nsource: https://sapling.ai/docs/api/api-access/\nschemes:\n  - type: apiKey\n    name: key\n    in: query\n    description: API key as query parameter\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: API key as Bearer token in Authorization header\n"
source_yaml_url: https://artifacts.apis.io/sapling/authentication/sapling-authentication.yml
summary_line: 2 schemes
tags:
- AI
- Language-Model
- API
- Enterprise
- Productivity
---
