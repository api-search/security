---
api_key_in:
- header
api_specs:
- filename: scansource-product-openapi.yml
  format: yaml
  label: ScanSource Product API
  slug: scansource-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scansource/refs/heads/main/openapi/scansource-product-openapi.yml
- filename: scansource-sales-order-openapi.yml
  format: yaml
  label: ScanSource Sales Order API
  slug: scansource-sales-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scansource/refs/heads/main/openapi/scansource-sales-order-openapi.yml
- filename: scansource-invoice-openapi.yml
  format: yaml
  label: ScanSource Invoice API
  slug: scansource-invoice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scansource/refs/heads/main/openapi/scansource-invoice-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Scansource Authentication
name_suffix: Authentication
oauth_flows: []
overview: ScanSource secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ScanSource
provider_slug: scansource
scheme_count: 1
schemes:
- description: Azure API Management subscription key from ScanSource partner portal
  in: header
  name: ApiKeyAuth
  parameter: Ocp-Apim-Subscription-Key
  sources:
  - openapi/scansource-invoice-openapi.yml
  - openapi/scansource-product-openapi.yml
  - openapi/scansource-sales-order-openapi.yml
  type: apiKey
slug: scansource-authentication
source_filename: scansource-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/scansource-invoice-openapi.yml, openapi/scansource-product-openapi.yml, openapi/scansource-sales-order-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Ocp-Apim-Subscription-Key\n  description: Azure API Management subscription key from ScanSource partner portal\n  sources:\n  - openapi/scansource-invoice-openapi.yml\n  - openapi/scansource-product-openapi.yml\n  - openapi/scansource-sales-order-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scansource/refs/heads/main/authentication/scansource-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- ScanSource
- Distribution
- Barcode
- Point Of Sale
- AIDC
- Inventory
- Order Management
- E-Commerce
- Fortune 1000
---
