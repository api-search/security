---
api_key_in:
- header
api_specs:
- filename: archrock-financials-api-openapi.yml
  format: yaml
  label: Archrock Financials API
  slug: archrock-financials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archrock/refs/heads/main/openapi/archrock-financials-api-openapi.yml
- filename: archrock-fleet-api-openapi.yml
  format: yaml
  label: Archrock Fleet API
  slug: archrock-fleet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archrock/refs/heads/main/openapi/archrock-fleet-api-openapi.yml
- filename: archrock-operations-api-openapi.yml
  format: yaml
  label: Archrock Operations API
  slug: archrock-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archrock/refs/heads/main/openapi/archrock-operations-api-openapi.yml
- filename: archrock-sec-filings-api-openapi.yml
  format: yaml
  label: Archrock SEC Filings API
  slug: archrock-sec-filings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archrock/refs/heads/main/openapi/archrock-sec-filings-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Archrock Authentication
name_suffix: Authentication
oauth_flows: []
overview: Archrock secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Archrock
provider_slug: archrock
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/archrock-investor-relations-api.yaml
  type: apiKey
slug: archrock-authentication
source_filename: archrock-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/archrock-investor-relations-api.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/archrock-investor-relations-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/archrock/refs/heads/main/authentication/archrock-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Natural Gas
- Compression Services
- Oil And Gas
- Energy
- Industrial
- 'NYSE: AROC'
---
