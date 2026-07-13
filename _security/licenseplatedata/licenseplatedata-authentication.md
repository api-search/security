---
api_key_in:
- header
api_specs:
- filename: licenseplatedata-openapi.yml
  format: yaml
  label: LicensePlateData
  slug: licenseplatedata
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/licenseplatedata/refs/heads/main/openapi/licenseplatedata-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Licenseplatedata Authentication
name_suffix: Authentication
oauth_flows: []
overview: LicensePlateData secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LicensePlateData
provider_slug: licenseplatedata
scheme_count: 1
schemes:
- in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/licenseplatedata-openapi.yml
  type: apiKey
slug: licenseplatedata-authentication
source_filename: licenseplatedata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/licenseplatedata-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/licenseplatedata-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/licenseplatedata/refs/heads/main/authentication/licenseplatedata-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Vehicles
- License Plates
- VIN
- Automotive
- Plate Lookup
- VIN Decoding
---
