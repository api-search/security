---
api_key_in:
- header
api_specs:
- filename: greenly-carbon-analytics-api-openapi.yml
  format: yaml
  label: Greenly Carbon Analytics API
  slug: greenly-carbon-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenly-earth/refs/heads/main/openapi/greenly-carbon-analytics-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Greenly Earth Authentication
name_suffix: Authentication
oauth_flows: []
overview: Greenly secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Greenly
provider_slug: greenly-earth
scheme_count: 1
schemes:
- in: header
  name: api_key
  parameter: api-key
  sources:
  - openapi/greenly-carbon-analytics-api-openapi.yml
  type: apiKey
slug: greenly-earth-authentication
source_filename: greenly-earth-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/greenly-carbon-analytics-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: api-key\n  sources:\n  - openapi/greenly-carbon-analytics-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/greenly-earth/refs/heads/main/authentication/greenly-earth-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Carbon Accounting
- Carbon Footprint
- Carbon Analytics
- Greenhouse Gas
- GHG Protocol
- Scope 1
- Scope 2
- Scope 3
- Sustainability
- ESG
- Climate
- CSRD
- CBAM
- EUDR
- SBTi
- TCFD
- EcoVadis
- Bilan Carbone
- Life Cycle Assessment
- Carbon Offsets
- SMB
- Fintech
- Transaction Enrichment
---
