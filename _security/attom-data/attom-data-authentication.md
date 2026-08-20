---
api_key_in:
- header
api_specs:
- filename: attom-data-area-api-openapi.yml
  format: yaml
  label: ATTOM Area API
  slug: attom-data-area-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attom-data/refs/heads/main/openapi/attom-data-area-api-openapi.yml
- filename: attom-data-assessment-api-openapi.yml
  format: yaml
  label: ATTOM Assessment API
  slug: attom-data-assessment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attom-data/refs/heads/main/openapi/attom-data-assessment-api-openapi.yml
- filename: attom-data-community-api-openapi.yml
  format: yaml
  label: ATTOM Community API
  slug: attom-data-community-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attom-data/refs/heads/main/openapi/attom-data-community-api-openapi.yml
- filename: attom-data-events-api-openapi.yml
  format: yaml
  label: ATTOM Events API
  slug: attom-data-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attom-data/refs/heads/main/openapi/attom-data-events-api-openapi.yml
- filename: attom-data-home-equity-api-openapi.yml
  format: yaml
  label: ATTOM Home Equity API
  slug: attom-data-home-equity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attom-data/refs/heads/main/openapi/attom-data-home-equity-api-openapi.yml
- filename: attom-data-mortgage-api-openapi.yml
  format: yaml
  label: ATTOM Mortgage API
  slug: attom-data-mortgage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attom-data/refs/heads/main/openapi/attom-data-mortgage-api-openapi.yml
- filename: attom-data-poi-api-openapi.yml
  format: yaml
  label: ATTOM POI API
  slug: attom-data-poi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attom-data/refs/heads/main/openapi/attom-data-poi-api-openapi.yml
- filename: attom-data-property-api-openapi.yml
  format: yaml
  label: ATTOM Property API
  slug: attom-data-property-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attom-data/refs/heads/main/openapi/attom-data-property-api-openapi.yml
- filename: attom-data-sales-api-openapi.yml
  format: yaml
  label: ATTOM Sales API
  slug: attom-data-sales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attom-data/refs/heads/main/openapi/attom-data-sales-api-openapi.yml
- filename: attom-data-school-api-openapi.yml
  format: yaml
  label: ATTOM School API
  slug: attom-data-school-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attom-data/refs/heads/main/openapi/attom-data-school-api-openapi.yml
- filename: attom-data-transportation-noise-api-openapi.yml
  format: yaml
  label: ATTOM Transportation Noise API
  slug: attom-data-transportation-noise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attom-data/refs/heads/main/openapi/attom-data-transportation-noise-api-openapi.yml
- filename: attom-data-valuation-api-openapi.yml
  format: yaml
  label: ATTOM Valuation API
  slug: attom-data-valuation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attom-data/refs/heads/main/openapi/attom-data-valuation-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Attom Data Authentication
name_suffix: Authentication
oauth_flows: []
overview: ATTOM secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ATTOM
provider_slug: attom-data
scheme_count: 1
schemes:
- description: 'Your unique ATTOM API key, assigned by ATTOM and passed in the `apikey` request header. Also send `Accept: application/json` (or application/xml).'
  in: header
  name: apiKeyAuth
  parameter: apikey
  sources:
  - openapi/attom-data-openapi.yml
  type: apiKey
slug: attom-data-authentication
source_filename: attom-data-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/attom-data-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: apikey\n  description: 'Your unique ATTOM API key, assigned by ATTOM and passed in the `apikey` request\n    header. Also send `Accept: application/json` (or application/xml).'\n  sources:\n  - openapi/attom-data-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/attom-data/refs/heads/main/authentication/attom-data-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Property Data
- Real-Estate
- Location Data
- Valuation
- AVM
- Assessment
- Mortgage
- Neighborhood
---
