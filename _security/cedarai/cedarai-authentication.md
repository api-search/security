---
api_key_in:
- header
api_specs:
- filename: cedarai-chargeservice-api-openapi.yml
  format: yaml
  label: Cedarai ChargeService API
  slug: cedarai-chargeservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cedarai/refs/heads/main/openapi/cedarai-chargeservice-api-openapi.yml
- filename: cedarai-equipment-history-api-openapi.yml
  format: yaml
  label: Cedarai Equipment History API
  slug: cedarai-equipment-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cedarai/refs/heads/main/openapi/cedarai-equipment-history-api-openapi.yml
- filename: cedarai-ims-api-openapi.yml
  format: yaml
  label: Cedarai Ims API
  slug: cedarai-ims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cedarai/refs/heads/main/openapi/cedarai-ims-api-openapi.yml
- filename: cedarai-invoicesservice-api-openapi.yml
  format: yaml
  label: Cedarai InvoicesService API
  slug: cedarai-invoicesservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cedarai/refs/heads/main/openapi/cedarai-invoicesservice-api-openapi.yml
- filename: cedarai-lindaservice-api-openapi.yml
  format: yaml
  label: Cedarai LindaService API
  slug: cedarai-lindaservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cedarai/refs/heads/main/openapi/cedarai-lindaservice-api-openapi.yml
- filename: cedarai-networkstructureservice-api-openapi.yml
  format: yaml
  label: Cedarai NetworkStructureService API
  slug: cedarai-networkstructureservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cedarai/refs/heads/main/openapi/cedarai-networkstructureservice-api-openapi.yml
- filename: cedarai-quotesservice-api-openapi.yml
  format: yaml
  label: Cedarai QuotesService API
  slug: cedarai-quotesservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cedarai/refs/heads/main/openapi/cedarai-quotesservice-api-openapi.yml
- filename: cedarai-truckloadtenderservice-api-openapi.yml
  format: yaml
  label: Cedarai TruckLoadTenderService API
  slug: cedarai-truckloadtenderservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cedarai/refs/heads/main/openapi/cedarai-truckloadtenderservice-api-openapi.yml
- filename: cedarai-workorderservice-api-openapi.yml
  format: yaml
  label: Cedarai WorkOrderService API
  slug: cedarai-workorderservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cedarai/refs/heads/main/openapi/cedarai-workorderservice-api-openapi.yml
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
