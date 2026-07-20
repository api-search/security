---
api_key_in:
- header
api_specs:
- filename: algodriven-vehicle-history-openapi.yml
  format: yaml
  label: Vehicle History Report - UAE
  slug: vehicle-history-report-uae
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algodriven/refs/heads/main/openapi/algodriven-vehicle-history-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Algodriven Authentication
name_suffix: Authentication
oauth_flows: []
overview: AlgoDriven secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AlgoDriven
provider_slug: algodriven
scheme_count: 1
schemes:
- description: API key passed in the Authorization request header.
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/algodriven-vehicle-history-openapi.yml
  type: apiKey
slug: algodriven-authentication
source_filename: algodriven-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: derived\nsource: openapi/algodriven-vehicle-history-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key passed in the Authorization request header.\n  sources:\n  - openapi/algodriven-vehicle-history-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/algodriven/refs/heads/main/authentication/algodriven-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Automotive
- Vehicle Data
- Car Valuation
- Vehicle Inspection
- Artificial Intelligence
- Vehicle History
- Automotive Data Intelligence
---
