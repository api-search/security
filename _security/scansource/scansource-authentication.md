---
api_key_in:
- header
api_specs:
- filename: scansource-availability-api-openapi.yml
  format: yaml
  label: ScanSource Availability API
  slug: scansource-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scansource/refs/heads/main/openapi/scansource-availability-api-openapi.yml
- filename: scansource-invoices-api-openapi.yml
  format: yaml
  label: ScanSource Invoices API
  slug: scansource-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scansource/refs/heads/main/openapi/scansource-invoices-api-openapi.yml
- filename: scansource-orders-api-openapi.yml
  format: yaml
  label: ScanSource Orders API
  slug: scansource-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scansource/refs/heads/main/openapi/scansource-orders-api-openapi.yml
- filename: scansource-pricing-api-openapi.yml
  format: yaml
  label: ScanSource Pricing API
  slug: scansource-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scansource/refs/heads/main/openapi/scansource-pricing-api-openapi.yml
- filename: scansource-products-api-openapi.yml
  format: yaml
  label: ScanSource Products API
  slug: scansource-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scansource/refs/heads/main/openapi/scansource-products-api-openapi.yml
- filename: scansource-shipping-api-openapi.yml
  format: yaml
  label: ScanSource Shipping API
  slug: scansource-shipping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scansource/refs/heads/main/openapi/scansource-shipping-api-openapi.yml
- filename: scansource-tracking-api-openapi.yml
  format: yaml
  label: ScanSource Tracking API
  slug: scansource-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scansource/refs/heads/main/openapi/scansource-tracking-api-openapi.yml
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
