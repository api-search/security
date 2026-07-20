---
api_key_in:
- header
api_specs:
- filename: cedarai-external-openapi.yml
  format: yaml
  label: Cedar ARMS External API
  slug: cedar-arms-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cedarai/refs/heads/main/openapi/cedarai-external-openapi.yml
- filename: cedarai-work-order-openapi.yml
  format: yaml
  label: Cedar ARMS Work Order API
  slug: cedar-arms-work-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cedarai/refs/heads/main/openapi/cedarai-work-order-openapi.yml
- filename: cedarai-charge-openapi.yml
  format: yaml
  label: Cedar ARMS Charges API
  slug: cedar-arms-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cedarai/refs/heads/main/openapi/cedarai-charge-openapi.yml
- filename: cedarai-invoices-openapi.yml
  format: yaml
  label: Cedar ARMS Shipper Invoices API
  slug: cedar-arms-shipper-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cedarai/refs/heads/main/openapi/cedarai-invoices-openapi.yml
- filename: cedarai-quotes-openapi.yml
  format: yaml
  label: Cedar ARMS Shipper Quotes API
  slug: cedar-arms-shipper-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cedarai/refs/heads/main/openapi/cedarai-quotes-openapi.yml
- filename: cedarai-load-tender-openapi.yml
  format: yaml
  label: Cedar ARMS Truck Load Tender API
  slug: cedar-arms-truck-load-tender-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cedarai/refs/heads/main/openapi/cedarai-load-tender-openapi.yml
- filename: cedarai-network-structure-openapi.yml
  format: yaml
  label: Cedar ARMS Network Structure API
  slug: cedar-arms-network-structure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cedarai/refs/heads/main/openapi/cedarai-network-structure-openapi.yml
- filename: cedarai-linda-notes-openapi.yml
  format: yaml
  label: Cedar Linda Notes API
  slug: cedar-linda-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cedarai/refs/heads/main/openapi/cedarai-linda-notes-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cedarai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cedarai secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cedarai
provider_slug: cedarai
scheme_count: 2
schemes:
- in: header
  name: ApiKeyAuth
  parameter: x-arms-api-key
  sources:
  - openapi/cedarai-charge-openapi.yml
  - openapi/cedarai-external-openapi.yml
  - openapi/cedarai-invoices-openapi.yml
  - openapi/cedarai-linda-notes-openapi.yml
  - openapi/cedarai-load-tender-openapi.yml
  - openapi/cedarai-network-structure-openapi.yml
  - openapi/cedarai-quotes-openapi.yml
  - openapi/cedarai-work-order-openapi.yml
  type: apiKey
- in: header
  name: AssumeUserAuth
  parameter: x-arms-assume-user
  sources:
  - openapi/cedarai-charge-openapi.yml
  - openapi/cedarai-external-openapi.yml
  - openapi/cedarai-invoices-openapi.yml
  - openapi/cedarai-linda-notes-openapi.yml
  - openapi/cedarai-load-tender-openapi.yml
  - openapi/cedarai-network-structure-openapi.yml
  - openapi/cedarai-quotes-openapi.yml
  - openapi/cedarai-work-order-openapi.yml
  type: apiKey
slug: cedarai-authentication
source_filename: cedarai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/cedarai-charge-openapi.yml, openapi/cedarai-external-openapi.yml, openapi/cedarai-invoices-openapi.yml,\n  openapi/cedarai-linda-notes-openapi.yml, openapi/cedarai-load-tender-openapi.yml, openapi/cedarai-network-structure-openapi.yml,\n  openapi/cedarai-quotes-openapi.yml, openapi/cedarai-work-order-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-arms-api-key\n  sources:\n  - openapi/cedarai-charge-openapi.yml\n  - openapi/cedarai-external-openapi.yml\n  - openapi/cedarai-invoices-openapi.yml\n  - openapi/cedarai-linda-notes-openapi.yml\n  - openapi/cedarai-load-tender-openapi.yml\n  - openapi/cedarai-network-structure-openapi.yml\n  - openapi/cedarai-quotes-openapi.yml\n  - openapi/cedarai-work-order-openapi.yml\n- name: AssumeUserAuth\n  type: apiKey\n  in: header\n  parameter: x-arms-assume-user\n  sources:\n  - openapi/cedarai-charge-openapi.yml\n\
  \  - openapi/cedarai-external-openapi.yml\n  - openapi/cedarai-invoices-openapi.yml\n  - openapi/cedarai-linda-notes-openapi.yml\n  - openapi/cedarai-load-tender-openapi.yml\n  - openapi/cedarai-network-structure-openapi.yml\n  - openapi/cedarai-quotes-openapi.yml\n  - openapi/cedarai-work-order-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cedarai/refs/heads/main/authentication/cedarai-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Rail
- Transportation
- Logistics
- Freight
- Supply Chain
- Railcar Management
- Transportation Management System
- Fleet Management
- Artificial Intelligence
---
