---
anonymous_access: false
api_key_in: []
api_specs:
- filename: arcadia-power-accounts-api-openapi.yml
  format: yaml
  label: Arcadia Accounts API
  slug: arcadia-power-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcadia-power/openapi/arcadia-power-accounts-api-openapi.yml
- filename: arcadia-power-credentials-api-openapi.yml
  format: yaml
  label: Arcadia Credentials API
  slug: arcadia-power-credentials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcadia-power/openapi/arcadia-power-credentials-api-openapi.yml
- filename: arcadia-power-files-api-openapi.yml
  format: yaml
  label: Arcadia Files API
  slug: arcadia-power-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcadia-power/openapi/arcadia-power-files-api-openapi.yml
- filename: arcadia-power-intervals-api-openapi.yml
  format: yaml
  label: Arcadia Intervals API
  slug: arcadia-power-intervals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcadia-power/openapi/arcadia-power-intervals-api-openapi.yml
- filename: arcadia-power-meters-api-openapi.yml
  format: yaml
  label: Arcadia Meters API
  slug: arcadia-power-meters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcadia-power/openapi/arcadia-power-meters-api-openapi.yml
- filename: arcadia-power-providers-api-openapi.yml
  format: yaml
  label: Arcadia Providers API
  slug: arcadia-power-providers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcadia-power/openapi/arcadia-power-providers-api-openapi.yml
- filename: arcadia-power-sites-api-openapi.yml
  format: yaml
  label: Arcadia Sites API
  slug: arcadia-power-sites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcadia-power/openapi/arcadia-power-sites-api-openapi.yml
- filename: arcadia-power-statements-api-openapi.yml
  format: yaml
  label: Arcadia Statements API
  slug: arcadia-power-statements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcadia-power/openapi/arcadia-power-statements-api-openapi.yml
- filename: arcadia-power-webhooks-api-openapi.yml
  format: yaml
  label: Arcadia Webhooks API
  slug: arcadia-power-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcadia-power/openapi/arcadia-power-webhooks-api-openapi.yml
- filename: arcadia-power-api-keys-api-openapi.yml
  format: yaml
  label: Arcadia API Keys API
  slug: arcadia-power-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcadia-power/openapi/arcadia-power-api-keys-api-openapi.yml
- filename: arcadia-power-authentication-api-openapi.yml
  format: yaml
  label: Arcadia Authentication API
  slug: arcadia-power-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcadia-power/openapi/arcadia-power-authentication-api-openapi.yml
- filename: arcadia-power-business-units-api-openapi.yml
  format: yaml
  label: Arcadia Business Units API
  slug: arcadia-power-business-units-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcadia-power/openapi/arcadia-power-business-units-api-openapi.yml
- filename: arcadia-power-custom-data-api-openapi.yml
  format: yaml
  label: Arcadia Custom Data API
  slug: arcadia-power-custom-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcadia-power/openapi/arcadia-power-custom-data-api-openapi.yml
- filename: arcadia-power-deletion-api-openapi.yml
  format: yaml
  label: Arcadia Deletion API
  slug: arcadia-power-deletion-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcadia-power/openapi/arcadia-power-deletion-api-openapi.yml
- filename: arcadia-power-discovered-statements-api-openapi.yml
  format: yaml
  label: Arcadia Discovered Statements API
  slug: arcadia-power-discovered-statements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcadia-power/openapi/arcadia-power-discovered-statements-api-openapi.yml
- filename: arcadia-power-downloads-api-openapi.yml
  format: yaml
  label: Arcadia Downloads API
  slug: arcadia-power-downloads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcadia-power/openapi/arcadia-power-downloads-api-openapi.yml
- filename: arcadia-power-expected-accounts-api-openapi.yml
  format: yaml
  label: Arcadia Expected Accounts API
  slug: arcadia-power-expected-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcadia-power/openapi/arcadia-power-expected-accounts-api-openapi.yml
- filename: arcadia-power-sandbox-statements-api-openapi.yml
  format: yaml
  label: Arcadia Sandbox Statements API
  slug: arcadia-power-sandbox-statements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcadia-power/openapi/arcadia-power-sandbox-statements-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Arcadia Power Authentication
name_suffix: Authentication
oauth_flows: []
overview: Arcadia secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Arcadia
provider_slug: arcadia-power
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/arcadia-plug-api-openapi.yml
  type: http
slug: arcadia-power-authentication
source_filename: arcadia-power-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/arcadia-plug-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/arcadia-plug-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/arcadia-power/authentication/arcadia-power-authentication.yml
summary_line: http · 1 scheme
tags:
- Energy
- Clean Energy
- Utility Data
- Climate
- Sustainability
- Carbon Accounting
- Solar
- Storage
- EV Charging
- Decarbonization
- Energy Intelligence
- Utilities
---
