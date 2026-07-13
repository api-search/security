---
api_key_in:
- header
api_specs:
- filename: finops-foundation-focus-cost-and-usage-openapi.yml
  format: yaml
  label: FOCUS Cost and Usage API
  slug: focus-cost-and-usage
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finops-foundation/refs/heads/main/openapi/finops-foundation-focus-cost-and-usage-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Finops Foundation Authentication
name_suffix: Authentication
oauth_flows: []
overview: FinOps Foundation secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: FinOps Foundation
provider_slug: finops-foundation
scheme_count: 2
schemes:
- description: Bearer token authentication for FOCUS API access.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/finops-foundation-focus-cost-and-usage-openapi.yml
  type: http
- description: API key authentication for FOCUS API access.
  in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/finops-foundation-focus-cost-and-usage-openapi.yml
  type: apiKey
slug: finops-foundation-authentication
source_filename: finops-foundation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/finops-foundation-focus-cost-and-usage-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication for FOCUS API access.\n  sources:\n  - openapi/finops-foundation-focus-cost-and-usage-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key authentication for FOCUS API access.\n  sources:\n  - openapi/finops-foundation-focus-cost-and-usage-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finops-foundation/refs/heads/main/authentication/finops-foundation-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Budgets
- Costs
- FinOps
---
