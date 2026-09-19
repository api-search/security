---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: equipmentwatch-bulk-api-openapi.yml
  format: yaml
  label: Equipmentwatch Bulk API
  slug: equipmentwatch-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equipmentwatch/refs/heads/main/openapi/equipmentwatch-bulk-api-openapi.yml
- filename: equipmentwatch-cost-api-openapi.yml
  format: yaml
  label: Equipmentwatch Cost API
  slug: equipmentwatch-cost-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equipmentwatch/refs/heads/main/openapi/equipmentwatch-cost-api-openapi.yml
- filename: equipmentwatch-rental-api-openapi.yml
  format: yaml
  label: Equipmentwatch Rental API
  slug: equipmentwatch-rental-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equipmentwatch/refs/heads/main/openapi/equipmentwatch-rental-api-openapi.yml
- filename: equipmentwatch-specifications-api-openapi.yml
  format: yaml
  label: Equipmentwatch Specifications API
  slug: equipmentwatch-specifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equipmentwatch/refs/heads/main/openapi/equipmentwatch-specifications-api-openapi.yml
- filename: equipmentwatch-taxonomy-api-openapi.yml
  format: yaml
  label: Equipmentwatch Taxonomy API
  slug: equipmentwatch-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equipmentwatch/refs/heads/main/openapi/equipmentwatch-taxonomy-api-openapi.yml
- filename: equipmentwatch-values-api-openapi.yml
  format: yaml
  label: Equipmentwatch Values API
  slug: equipmentwatch-values-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equipmentwatch/refs/heads/main/openapi/equipmentwatch-values-api-openapi.yml
- filename: equipmentwatch-verification-api-openapi.yml
  format: yaml
  label: Equipmentwatch Verification API
  slug: equipmentwatch-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equipmentwatch/refs/heads/main/openapi/equipmentwatch-verification-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Equipmentwatch Authentication
name_suffix: Authentication
oauth_flows: []
overview: Equipmentwatch secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Equipmentwatch
provider_slug: equipmentwatch
scheme_count: 1
schemes:
- in: header
  name: API Key
  parameter: x-api-key
  sources:
  - openapi/equipmentwatch-api-openapi.yaml
  type: apiKey
slug: equipmentwatch-authentication
source_filename: equipmentwatch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: derived\nsource: openapi/equipmentwatch-api-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: API Key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/equipmentwatch-api-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/equipmentwatch/refs/heads/main/authentication/equipmentwatch-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Construction
- Equipment
- Rental Rates
- Valuation
- Heavy Equipment
- Equipment Data
- Market Data
---
