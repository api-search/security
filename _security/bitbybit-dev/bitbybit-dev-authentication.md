---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bitbybit-dev-cad-operations-api-openapi.yml
  format: yaml
  label: bitbybit-dev CAD Operations API
  slug: bitbybit-dev-cad-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitbybit-dev/openapi/bitbybit-dev-cad-operations-api-openapi.yml
- filename: bitbybit-dev-convert-api-openapi.yml
  format: yaml
  label: bitbybit-dev Convert API
  slug: bitbybit-dev-convert-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitbybit-dev/openapi/bitbybit-dev-convert-api-openapi.yml
- filename: bitbybit-dev-files-api-openapi.yml
  format: yaml
  label: bitbybit-dev Files API
  slug: bitbybit-dev-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitbybit-dev/openapi/bitbybit-dev-files-api-openapi.yml
- filename: bitbybit-dev-health-api-openapi.yml
  format: yaml
  label: bitbybit-dev Health API
  slug: bitbybit-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitbybit-dev/openapi/bitbybit-dev-health-api-openapi.yml
- filename: bitbybit-dev-models-api-openapi.yml
  format: yaml
  label: bitbybit-dev Models API
  slug: bitbybit-dev-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitbybit-dev/openapi/bitbybit-dev-models-api-openapi.yml
- filename: bitbybit-dev-models-dragon-cup-api-openapi.yml
  format: yaml
  label: bitbybit-dev Models - Dragon Cup API
  slug: bitbybit-dev-models-dragon-cup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitbybit-dev/openapi/bitbybit-dev-models-dragon-cup-api-openapi.yml
- filename: bitbybit-dev-models-phone-nest-api-openapi.yml
  format: yaml
  label: bitbybit-dev Models - Phone Nest API
  slug: bitbybit-dev-models-phone-nest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitbybit-dev/openapi/bitbybit-dev-models-phone-nest-api-openapi.yml
- filename: bitbybit-dev-sheet-metal-api-openapi.yml
  format: yaml
  label: bitbybit-dev Sheet Metal API
  slug: bitbybit-dev-sheet-metal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitbybit-dev/openapi/bitbybit-dev-sheet-metal-api-openapi.yml
- filename: bitbybit-dev-tasks-api-openapi.yml
  format: yaml
  label: bitbybit-dev Tasks API
  slug: bitbybit-dev-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitbybit-dev/openapi/bitbybit-dev-tasks-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Bitbybit Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: bitbybit-dev declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: bitbybit-dev
provider_slug: bitbybit-dev
scheme_count: 1
schemes:
- description: 'Scoped API key. Scopes: models, cad, convert, * (wildcard). A key without the required scope receives 403 INSUFFICIENT_SCOPE.'
  in: header
  name: X-API-Key
  type: apiKey
slug: bitbybit-dev-authentication
source_filename: bitbybit-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/bitbybit-dev-openapi.json\nschemes:\n  - type: apiKey\n    in: header\n    name: X-API-Key\n    description: \"Scoped API key. Scopes: models, cad, convert, * (wildcard). A key without the required scope receives 403 INSUFFICIENT_SCOPE.\"\n"
source_yaml_url: https://artifacts.apis.io/bitbybit-dev/authentication/bitbybit-dev-authentication.yml
summary_line: 1 scheme
tags:
- 3D CAD
- TypeScript
- API
- Platform
- Creative Coding
- Modeling
---
