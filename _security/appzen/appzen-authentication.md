---
api_key_in:
- header
api_specs:
- filename: appzen-chart-of-accounts-api-openapi.yml
  format: yaml
  label: AppZen Chart of Accounts API
  slug: appzen-chart-of-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appzen/refs/heads/main/openapi/appzen-chart-of-accounts-api-openapi.yml
- filename: appzen-custom-data-sets-api-openapi.yml
  format: yaml
  label: AppZen Custom Data Sets API
  slug: appzen-custom-data-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appzen/refs/heads/main/openapi/appzen-custom-data-sets-api-openapi.yml
- filename: appzen-documents-api-openapi.yml
  format: yaml
  label: AppZen Documents API
  slug: appzen-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appzen/refs/heads/main/openapi/appzen-documents-api-openapi.yml
- filename: appzen-entities-api-openapi.yml
  format: yaml
  label: AppZen Entities API
  slug: appzen-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appzen/refs/heads/main/openapi/appzen-entities-api-openapi.yml
- filename: appzen-externally-processed-invoices-api-openapi.yml
  format: yaml
  label: AppZen Externally Processed Invoices API
  slug: appzen-externally-processed-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appzen/refs/heads/main/openapi/appzen-externally-processed-invoices-api-openapi.yml
- filename: appzen-goods-receipt-api-openapi.yml
  format: yaml
  label: AppZen Goods Receipt API
  slug: appzen-goods-receipt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appzen/refs/heads/main/openapi/appzen-goods-receipt-api-openapi.yml
- filename: appzen-invoice-audit-results-api-openapi.yml
  format: yaml
  label: AppZen Invoice Audit Results API
  slug: appzen-invoice-audit-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appzen/refs/heads/main/openapi/appzen-invoice-audit-results-api-openapi.yml
- filename: appzen-invoice-status-sync-api-openapi.yml
  format: yaml
  label: AppZen Invoice Status Sync API
  slug: appzen-invoice-status-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appzen/refs/heads/main/openapi/appzen-invoice-status-sync-api-openapi.yml
- filename: appzen-invoices-api-openapi.yml
  format: yaml
  label: AppZen Invoices API
  slug: appzen-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appzen/refs/heads/main/openapi/appzen-invoices-api-openapi.yml
- filename: appzen-lookup-item-api-openapi.yml
  format: yaml
  label: AppZen Lookup Item API
  slug: appzen-lookup-item-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appzen/refs/heads/main/openapi/appzen-lookup-item-api-openapi.yml
- filename: appzen-lookup-table-api-openapi.yml
  format: yaml
  label: AppZen Lookup Table API
  slug: appzen-lookup-table-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appzen/refs/heads/main/openapi/appzen-lookup-table-api-openapi.yml
- filename: appzen-payment-terms-api-openapi.yml
  format: yaml
  label: AppZen Payment Terms API
  slug: appzen-payment-terms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appzen/refs/heads/main/openapi/appzen-payment-terms-api-openapi.yml
- filename: appzen-processed-invoices-api-openapi.yml
  format: yaml
  label: AppZen Processed Invoices API
  slug: appzen-processed-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appzen/refs/heads/main/openapi/appzen-processed-invoices-api-openapi.yml
- filename: appzen-purchase-orders-api-openapi.yml
  format: yaml
  label: AppZen Purchase Orders API
  slug: appzen-purchase-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appzen/refs/heads/main/openapi/appzen-purchase-orders-api-openapi.yml
- filename: appzen-suppliers-api-openapi.yml
  format: yaml
  label: AppZen Suppliers API
  slug: appzen-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appzen/refs/heads/main/openapi/appzen-suppliers-api-openapi.yml
- filename: appzen-tax-master-api-openapi.yml
  format: yaml
  label: AppZen Tax Master API
  slug: appzen-tax-master-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appzen/refs/heads/main/openapi/appzen-tax-master-api-openapi.yml
- filename: appzen-unit-of-measures-api-openapi.yml
  format: yaml
  label: AppZen Unit of Measures API
  slug: appzen-unit-of-measures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appzen/refs/heads/main/openapi/appzen-unit-of-measures-api-openapi.yml
- filename: appzen-user-groups-api-openapi.yml
  format: yaml
  label: AppZen User Groups API
  slug: appzen-user-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appzen/refs/heads/main/openapi/appzen-user-groups-api-openapi.yml
- filename: appzen-vat-api-openapi.yml
  format: yaml
  label: AppZen Vat API
  slug: appzen-vat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appzen/refs/heads/main/openapi/appzen-vat-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Appzen Authentication
name_suffix: Authentication
oauth_flows: []
overview: AppZen secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AppZen
provider_slug: appzen
scheme_count: 3
schemes:
- description: API key issued by AppZen Support.
  in: header
  name: API Key Header
  parameter: x-api-key
  sources:
  - openapi/appzen-autonomous-ap-openapi-original.yml
  type: apiKey
- description: Customer identifier issued by AppZen Support.
  in: header
  name: Customer Id Header
  parameter: customer-id
  sources:
  - openapi/appzen-autonomous-ap-openapi-original.yml
  type: apiKey
- description: Customer key issued by AppZen Support.
  in: header
  name: Customer Key Header
  parameter: customer-key
  sources:
  - openapi/appzen-autonomous-ap-openapi-original.yml
  type: apiKey
slug: appzen-authentication
source_filename: appzen-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/appzen-autonomous-ap-openapi-original.yml\ndocs: https://support.appzen.com/hc/en-us/articles/12905088759571-Authentication-Overview\nguidelines: https://api-docs.appzen.com/api_guidelines.html\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  notes: >-\n    AppZen's Autonomous AP public APIs use API-key header authentication. Three\n    values, all issued by the AppZen Support team, must be sent on every request:\n    x-api-key, customer-id, and customer-key. The docs describe the model as\n    \"API key-based authentication (OAuth1.0)\". Every response returns an\n    x-correlation-id header to be quoted to AppZen support when troubleshooting.\nschemes:\n- name: API Key Header\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key issued by AppZen Support.\n  sources:\n  - openapi/appzen-autonomous-ap-openapi-original.yml\n- name: Customer Id Header\n  type: apiKey\n  in: header\n\
  \  parameter: customer-id\n  description: Customer identifier issued by AppZen Support.\n  sources:\n  - openapi/appzen-autonomous-ap-openapi-original.yml\n- name: Customer Key Header\n  type: apiKey\n  in: header\n  parameter: customer-key\n  description: Customer key issued by AppZen Support.\n  sources:\n  - openapi/appzen-autonomous-ap-openapi-original.yml\nresponse_headers:\n- name: x-correlation-id\n  description: Present on every response (success and failure); provide to AppZen Support for troubleshooting.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appzen/refs/heads/main/authentication/appzen-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Finance
- Accounts Payable
- Expense Management
- Invoice Processing
- Spend Audit
- Artificial Intelligence
- ERP Integration
---
