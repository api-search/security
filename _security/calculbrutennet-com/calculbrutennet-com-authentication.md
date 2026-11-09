---
anonymous_access: false
api_key_in: []
api_specs:
- filename: calculbrutennet-com-dataset-api-openapi.yml
  format: yaml
  label: Calcul Brut en Net Dataset API
  slug: calculbrutennet-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calculbrutennet-com/openapi/calculbrutennet-com-dataset-api-openapi.yml
- filename: calculbrutennet-com-enquiry-api-openapi.yml
  format: yaml
  label: Calcul Brut en Net Enquiry API
  slug: calculbrutennet-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calculbrutennet-com/openapi/calculbrutennet-com-enquiry-api-openapi.yml
- filename: calculbrutennet-com-mcp-api-openapi.yml
  format: yaml
  label: Calcul Brut en Net MCP API
  slug: calculbrutennet-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calculbrutennet-com/openapi/calculbrutennet-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Calculbrutennet Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Calcul Brut en Net secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Calcul Brut en Net
provider_slug: calculbrutennet-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/calculbrutennet-com-openapi.json
  type: http
slug: calculbrutennet-com-authentication
source_filename: calculbrutennet-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: derived\nsource: openapi/calculbrutennet-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/calculbrutennet-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/calculbrutennet-com/authentication/calculbrutennet-com-authentication.yml
summary_line: http · 1 scheme
tags:
- French
- Payroll
- Social Security
- Labor Law
- CalculBrutEnNet
- Company
---
