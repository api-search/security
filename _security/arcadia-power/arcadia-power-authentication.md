---
api_key_in: []
api_specs:
- filename: arcadia-power-accounts-api-openapi.yml
  format: yaml
  label: Arcadia Accounts API
  slug: arcadia-power-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadia-power/refs/heads/main/openapi/arcadia-power-accounts-api-openapi.yml
- filename: arcadia-power-credentials-api-openapi.yml
  format: yaml
  label: Arcadia Credentials API
  slug: arcadia-power-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadia-power/refs/heads/main/openapi/arcadia-power-credentials-api-openapi.yml
- filename: arcadia-power-files-api-openapi.yml
  format: yaml
  label: Arcadia Files API
  slug: arcadia-power-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadia-power/refs/heads/main/openapi/arcadia-power-files-api-openapi.yml
- filename: arcadia-power-intervals-api-openapi.yml
  format: yaml
  label: Arcadia Intervals API
  slug: arcadia-power-intervals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadia-power/refs/heads/main/openapi/arcadia-power-intervals-api-openapi.yml
- filename: arcadia-power-meters-api-openapi.yml
  format: yaml
  label: Arcadia Meters API
  slug: arcadia-power-meters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadia-power/refs/heads/main/openapi/arcadia-power-meters-api-openapi.yml
- filename: arcadia-power-oauth-api-openapi.yml
  format: yaml
  label: Arcadia OAuth API
  slug: arcadia-power-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadia-power/refs/heads/main/openapi/arcadia-power-oauth-api-openapi.yml
- filename: arcadia-power-organizations-api-openapi.yml
  format: yaml
  label: Arcadia Organizations API
  slug: arcadia-power-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadia-power/refs/heads/main/openapi/arcadia-power-organizations-api-openapi.yml
- filename: arcadia-power-providers-api-openapi.yml
  format: yaml
  label: Arcadia Providers API
  slug: arcadia-power-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadia-power/refs/heads/main/openapi/arcadia-power-providers-api-openapi.yml
- filename: arcadia-power-sites-api-openapi.yml
  format: yaml
  label: Arcadia Sites API
  slug: arcadia-power-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadia-power/refs/heads/main/openapi/arcadia-power-sites-api-openapi.yml
- filename: arcadia-power-statements-api-openapi.yml
  format: yaml
  label: Arcadia Statements API
  slug: arcadia-power-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadia-power/refs/heads/main/openapi/arcadia-power-statements-api-openapi.yml
- filename: arcadia-power-webhooks-api-openapi.yml
  format: yaml
  label: Arcadia Webhooks API
  slug: arcadia-power-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadia-power/refs/heads/main/openapi/arcadia-power-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
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
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arcadia-power/refs/heads/main/authentication/arcadia-power-authentication.yml
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
---
