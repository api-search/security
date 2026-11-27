---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: arcnautical-com-account-api-openapi.yml
  format: yaml
  label: ArcNautical Account API
  slug: arcnautical-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnautical-com/openapi/arcnautical-com-account-api-openapi.yml
- filename: arcnautical-com-cargo-screening-api-openapi.yml
  format: yaml
  label: ArcNautical Cargo screening API
  slug: arcnautical-com-cargo-screening-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnautical-com/openapi/arcnautical-com-cargo-screening-api-openapi.yml
- filename: arcnautical-com-corridor-monitors-api-openapi.yml
  format: yaml
  label: ArcNautical Corridor monitors API
  slug: arcnautical-com-corridor-monitors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnautical-com/openapi/arcnautical-com-corridor-monitors-api-openapi.yml
- filename: arcnautical-com-crew-placement-api-openapi.yml
  format: yaml
  label: ArcNautical Crew placement API
  slug: arcnautical-com-crew-placement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnautical-com/openapi/arcnautical-com-crew-placement-api-openapi.yml
- filename: arcnautical-com-exports-api-openapi.yml
  format: yaml
  label: ArcNautical Exports API
  slug: arcnautical-com-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnautical-com/openapi/arcnautical-com-exports-api-openapi.yml
- filename: arcnautical-com-fleets-api-openapi.yml
  format: yaml
  label: ArcNautical Fleets API
  slug: arcnautical-com-fleets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnautical-com/openapi/arcnautical-com-fleets-api-openapi.yml
- filename: arcnautical-com-port-lookup-api-openapi.yml
  format: yaml
  label: ArcNautical Port lookup API
  slug: arcnautical-com-port-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnautical-com/openapi/arcnautical-com-port-lookup-api-openapi.yml
- filename: arcnautical-com-public-vessel-check-api-openapi.yml
  format: yaml
  label: ArcNautical Public vessel check API
  slug: arcnautical-com-public-vessel-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnautical-com/openapi/arcnautical-com-public-vessel-check-api-openapi.yml
- filename: arcnautical-com-vessel-monitors-api-openapi.yml
  format: yaml
  label: ArcNautical Vessel monitors API
  slug: arcnautical-com-vessel-monitors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnautical-com/openapi/arcnautical-com-vessel-monitors-api-openapi.yml
- filename: arcnautical-com-vessel-screening-api-openapi.yml
  format: yaml
  label: ArcNautical Vessel screening API
  slug: arcnautical-com-vessel-screening-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnautical-com/openapi/arcnautical-com-vessel-screening-api-openapi.yml
- filename: arcnautical-com-voyage-assessments-api-openapi.yml
  format: yaml
  label: ArcNautical Voyage assessments API
  slug: arcnautical-com-voyage-assessments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnautical-com/openapi/arcnautical-com-voyage-assessments-api-openapi.yml
- filename: arcnautical-com-webhooks-api-openapi.yml
  format: yaml
  label: ArcNautical Webhooks API
  slug: arcnautical-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnautical-com/openapi/arcnautical-com-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: ArcNautical Authentication
name_suffix: Authentication
oauth_flows: []
overview: ArcNautical secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ArcNautical
provider_slug: arcnautical-com
scheme_count: 2
schemes:
- bearerFormat: arc_live_... or arc_test_...
  description: 'Preferred authentication. Use Authorization: Bearer arc_live_... or arc_test_....'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/arcnautical-com-openapi.json
  type: http
- description: Compatibility header for customers that cannot send Bearer tokens.
  in: header
  name: legacyApiKey
  parameter: X-ArcNautical-Key
  sources:
  - openapi/arcnautical-com-openapi.json
  type: apiKey
slug: arcnautical-com-authentication
source_filename: arcnautical-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: openapi/arcnautical-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: arc_live_... or arc_test_...\n  description: 'Preferred authentication. Use Authorization: Bearer arc_live_... or arc_test_....'\n  sources:\n  - openapi/arcnautical-com-openapi.json\n- name: legacyApiKey\n  type: apiKey\n  in: header\n  parameter: X-ArcNautical-Key\n  description: Compatibility header for customers that cannot send Bearer tokens.\n  sources:\n  - openapi/arcnautical-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/arcnautical-com/authentication/arcnautical-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Maritime
- Compliance
- Data
- Screening
---
