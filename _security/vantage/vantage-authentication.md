---
api_key_in: []
api_specs:
- filename: vantage-cost-management-api-openapi.yml
  format: yaml
  label: Vantage Cost Management API
  slug: cost-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/openapi/vantage-cost-management-api-openapi.yml
- filename: vantage-cloud-pricing-api-openapi.yml
  format: yaml
  label: Vantage Cloud Pricing API
  slug: cloud-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/openapi/vantage-cloud-pricing-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Vantage Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vantage secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vantage
provider_slug: vantage
scheme_count: 1
schemes:
- description: Vantage API token. Create a free API key from your Vantage account page at https://console.vantage.sh/account/api_access_tokens.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/vantage-cloud-pricing-api-openapi.yml
  - openapi/vantage-cost-management-api-openapi.yml
  type: http
slug: vantage-authentication
source_filename: vantage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vantage-cloud-pricing-api-openapi.yml, openapi/vantage-cost-management-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Vantage API token. Create a free API key from your Vantage account page at https://console.vantage.sh/account/api_access_tokens.\n  sources:\n  - openapi/vantage-cloud-pricing-api-openapi.yml\n  - openapi/vantage-cost-management-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/authentication/vantage-authentication.yml
summary_line: http · 1 scheme
tags:
- Budgets
- Cloud Pricing
- Cost Management
- Costs
- FinOps
---
