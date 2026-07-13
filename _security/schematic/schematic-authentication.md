---
api_key_in:
- header
api_specs:
- filename: schematic-openapi.yml
  format: yaml
  label: Schematic API
  slug: schematic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schematic/refs/heads/main/openapi/schematic-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Schematic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Schematic secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Schematic
provider_slug: schematic
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-Schematic-Api-Key
  sources:
  - openapi/schematic-openapi.yml
  type: apiKey
slug: schematic-authentication
source_filename: schematic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/schematic-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Schematic-Api-Key\n  sources:\n  - openapi/schematic-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/schematic/refs/heads/main/authentication/schematic-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Billing
- Entitlements
- Feature Flags
- Feature Management
- FinOps
- Metering
- Pricing
- SaaS
---
