---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: equipmentwatch-api-openapi.yaml
  format: yaml
  label: EquipmentWatch Taxonomy API
  slug: taxonomy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equipmentwatch/refs/heads/main/openapi/equipmentwatch-api-openapi.yaml
- filename: equipmentwatch-api-openapi.yaml
  format: yaml
  label: EquipmentWatch Specs API
  slug: specs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equipmentwatch/refs/heads/main/openapi/equipmentwatch-api-openapi.yaml
- filename: equipmentwatch-api-openapi.yaml
  format: yaml
  label: EquipmentWatch Verification API
  slug: verification
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equipmentwatch/refs/heads/main/openapi/equipmentwatch-api-openapi.yaml
- filename: equipmentwatch-api-openapi.yaml
  format: yaml
  label: EquipmentWatch Costs API
  slug: costs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equipmentwatch/refs/heads/main/openapi/equipmentwatch-api-openapi.yaml
- filename: equipmentwatch-api-openapi.yaml
  format: yaml
  label: EquipmentWatch Values API
  slug: values
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equipmentwatch/refs/heads/main/openapi/equipmentwatch-api-openapi.yaml
- filename: equipmentwatch-api-openapi.yaml
  format: yaml
  label: EquipmentWatch Retail Rental API
  slug: retail-rental
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equipmentwatch/refs/heads/main/openapi/equipmentwatch-api-openapi.yaml
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
