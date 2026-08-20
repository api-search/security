---
api_key_in:
- header
api_specs:
- filename: nory-authorization-api-openapi.yml
  format: yaml
  label: Nory Authorization API
  slug: nory-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nory/refs/heads/main/openapi/nory-authorization-api-openapi.yml
- filename: nory-branch-api-openapi.yml
  format: yaml
  label: Nory Branch API
  slug: nory-branch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nory/refs/heads/main/openapi/nory-branch-api-openapi.yml
- filename: nory-brands-api-openapi.yml
  format: yaml
  label: Nory Brands API
  slug: nory-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nory/refs/heads/main/openapi/nory-brands-api-openapi.yml
- filename: nory-employee-punch-api-openapi.yml
  format: yaml
  label: Nory Employee Punch API
  slug: nory-employee-punch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nory/refs/heads/main/openapi/nory-employee-punch-api-openapi.yml
- filename: nory-integration-api-openapi.yml
  format: yaml
  label: Nory Integration API
  slug: nory-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nory/refs/heads/main/openapi/nory-integration-api-openapi.yml
- filename: nory-inventory-api-openapi.yml
  format: yaml
  label: Nory Inventory API
  slug: nory-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nory/refs/heads/main/openapi/nory-inventory-api-openapi.yml
- filename: nory-inventory-orders-api-openapi.yml
  format: yaml
  label: Nory Inventory Orders API
  slug: nory-inventory-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nory/refs/heads/main/openapi/nory-inventory-orders-api-openapi.yml
- filename: nory-location-settings-api-openapi.yml
  format: yaml
  label: Nory Location Settings API
  slug: nory-location-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nory/refs/heads/main/openapi/nory-location-settings-api-openapi.yml
- filename: nory-refresh-token-api-openapi.yml
  format: yaml
  label: Nory Refresh token API
  slug: nory-refresh-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nory/refs/heads/main/openapi/nory-refresh-token-api-openapi.yml
- filename: nory-templates-api-openapi.yml
  format: yaml
  label: Nory Templates API
  slug: nory-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nory/refs/heads/main/openapi/nory-templates-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Nory Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nory secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nory
provider_slug: nory
scheme_count: 1
schemes:
- in: header
  name: bearerAuth
  parameter: Authorization
  sources:
  - openapi/nory-middleware-openapi.json
  type: apiKey
slug: nory-authentication
source_filename: nory-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/nory-middleware-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/nory-middleware-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nory/refs/heads/main/authentication/nory-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Restaurant
- Hospitality
- Inventory
- Workforce
- Payroll
- Point-of-Sale
- Artificial Intelligence
- Food and Beverage
---
