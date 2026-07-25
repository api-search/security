---
api_key_in:
- header
api_specs:
- filename: telefono-batch-api-openapi.yml
  format: yaml
  label: Telefono Batch API
  slug: telefono-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefono/refs/heads/main/openapi/telefono-batch-api-openapi.yml
- filename: telefono-carrier-api-openapi.yml
  format: yaml
  label: Telefono Carrier API
  slug: telefono-carrier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefono/refs/heads/main/openapi/telefono-carrier-api-openapi.yml
- filename: telefono-format-api-openapi.yml
  format: yaml
  label: Telefono Format API
  slug: telefono-format-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefono/refs/heads/main/openapi/telefono-format-api-openapi.yml
- filename: telefono-validation-api-openapi.yml
  format: yaml
  label: Telefono Validation API
  slug: telefono-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefono/refs/heads/main/openapi/telefono-validation-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Telefono Authentication
name_suffix: Authentication
oauth_flows: []
overview: Telefono secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Telefono
provider_slug: telefono
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/telefono-carrier-openapi.yml
  - openapi/telefono-format-openapi.yml
  - openapi/telefono-validation-openapi.yml
  type: apiKey
slug: telefono-authentication
source_filename: telefono-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/telefono-carrier-openapi.yml, openapi/telefono-format-openapi.yml, openapi/telefono-validation-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/telefono-carrier-openapi.yml\n  - openapi/telefono-format-openapi.yml\n  - openapi/telefono-validation-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telefono/refs/heads/main/authentication/telefono-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Carrier Lookup
- Data Enrichment
- Fraud Prevention
- Number Intelligence
- Number Verification
- Phone Lookup
- Phone Validation
- Telecommunications
---
