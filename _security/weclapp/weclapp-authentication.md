---
api_key_in: []
api_specs:
- filename: weclapp-openapi.yml
  format: yaml
  label: weclapp Customer API
  slug: weclapp-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weclapp/refs/heads/main/openapi/weclapp-openapi.yml
- filename: weclapp-openapi.yml
  format: yaml
  label: weclapp Article API
  slug: weclapp-article-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weclapp/refs/heads/main/openapi/weclapp-openapi.yml
- filename: weclapp-openapi.yml
  format: yaml
  label: weclapp Sales Order API
  slug: weclapp-sales-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weclapp/refs/heads/main/openapi/weclapp-openapi.yml
- filename: weclapp-openapi.yml
  format: yaml
  label: weclapp Quotation API
  slug: weclapp-quotation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weclapp/refs/heads/main/openapi/weclapp-openapi.yml
- filename: weclapp-openapi.yml
  format: yaml
  label: weclapp Sales Invoice API
  slug: weclapp-sales-invoice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weclapp/refs/heads/main/openapi/weclapp-openapi.yml
- filename: weclapp-openapi.yml
  format: yaml
  label: weclapp Shipment API
  slug: weclapp-shipment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weclapp/refs/heads/main/openapi/weclapp-openapi.yml
- filename: weclapp-openapi.yml
  format: yaml
  label: weclapp Purchase Order API
  slug: weclapp-purchase-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weclapp/refs/heads/main/openapi/weclapp-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Weclapp Authentication
name_suffix: Authentication
oauth_flows: []
overview: weclapp secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: weclapp
provider_slug: weclapp
scheme_count: 1
schemes:
- description: 'Per-user API token issued inside weclapp under "My Settings > API", sent in the `AuthenticationToken` request header (`AuthenticationToken: <token>`). This is not OAuth and not a Bearer token. Requests must also send `Accept: application/json`; `POST` and `PUT` requests must additionally send `Content-Type: application/json`.'
  in: header
  name: authenticationToken
  parameterName: AuthenticationToken
  sources:
  - openapi/weclapp-openapi.yml
  - https://www.weclapp.com/api/
  type: apiKey
slug: weclapp-authentication
source_filename: weclapp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/weclapp-openapi.yml\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: authenticationToken\n  type: apiKey\n  in: header\n  parameterName: AuthenticationToken\n  description: >-\n    Per-user API token issued inside weclapp under \"My Settings > API\", sent in\n    the `AuthenticationToken` request header (`AuthenticationToken: <token>`).\n    This is not OAuth and not a Bearer token. Requests must also send\n    `Accept: application/json`; `POST` and `PUT` requests must additionally send\n    `Content-Type: application/json`.\n  sources:\n  - openapi/weclapp-openapi.yml\n  - https://www.weclapp.com/api/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weclapp/refs/heads/main/authentication/weclapp-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- ERP
- CRM
- Cloud ERP
- Accounting
- Inventory
- Commerce
- Germany
- Order Management
- Business Software
- SaaS
---
