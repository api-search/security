---
api_key_in:
- query
api_specs:
- filename: prodsmart-authorization-api-openapi.yml
  format: yaml
  label: Prodsmart Authorization API
  slug: prodsmart-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodsmart/refs/heads/main/openapi/prodsmart-authorization-api-openapi.yml
- filename: prodsmart-changes-feed-api-openapi.yml
  format: yaml
  label: Prodsmart Changes Feed API
  slug: prodsmart-changes-feed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodsmart/refs/heads/main/openapi/prodsmart-changes-feed-api-openapi.yml
- filename: prodsmart-clients-api-openapi.yml
  format: yaml
  label: Prodsmart Clients API
  slug: prodsmart-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodsmart/refs/heads/main/openapi/prodsmart-clients-api-openapi.yml
- filename: prodsmart-downtime-api-openapi.yml
  format: yaml
  label: Prodsmart Downtime API
  slug: prodsmart-downtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodsmart/refs/heads/main/openapi/prodsmart-downtime-api-openapi.yml
- filename: prodsmart-inventory-api-openapi.yml
  format: yaml
  label: Prodsmart Inventory API
  slug: prodsmart-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodsmart/refs/heads/main/openapi/prodsmart-inventory-api-openapi.yml
- filename: prodsmart-machines-api-openapi.yml
  format: yaml
  label: Prodsmart Machines API
  slug: prodsmart-machines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodsmart/refs/heads/main/openapi/prodsmart-machines-api-openapi.yml
- filename: prodsmart-product-families-api-openapi.yml
  format: yaml
  label: Prodsmart Product Families API
  slug: prodsmart-product-families-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodsmart/refs/heads/main/openapi/prodsmart-product-families-api-openapi.yml
- filename: prodsmart-production-orders-api-openapi.yml
  format: yaml
  label: Prodsmart Production Orders API
  slug: prodsmart-production-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodsmart/refs/heads/main/openapi/prodsmart-production-orders-api-openapi.yml
- filename: prodsmart-productions-api-openapi.yml
  format: yaml
  label: Prodsmart Productions API
  slug: prodsmart-productions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodsmart/refs/heads/main/openapi/prodsmart-productions-api-openapi.yml
- filename: prodsmart-products-api-openapi.yml
  format: yaml
  label: Prodsmart Products API
  slug: prodsmart-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodsmart/refs/heads/main/openapi/prodsmart-products-api-openapi.yml
- filename: prodsmart-punch-clock-api-openapi.yml
  format: yaml
  label: Prodsmart Punch Clock API
  slug: prodsmart-punch-clock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodsmart/refs/heads/main/openapi/prodsmart-punch-clock-api-openapi.yml
- filename: prodsmart-purchase-orders-api-openapi.yml
  format: yaml
  label: Prodsmart Purchase Orders API
  slug: prodsmart-purchase-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodsmart/refs/heads/main/openapi/prodsmart-purchase-orders-api-openapi.yml
- filename: prodsmart-reports-api-openapi.yml
  format: yaml
  label: Prodsmart Reports API
  slug: prodsmart-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodsmart/refs/heads/main/openapi/prodsmart-reports-api-openapi.yml
- filename: prodsmart-sales-orders-api-openapi.yml
  format: yaml
  label: Prodsmart Sales Orders API
  slug: prodsmart-sales-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodsmart/refs/heads/main/openapi/prodsmart-sales-orders-api-openapi.yml
- filename: prodsmart-suppliers-api-openapi.yml
  format: yaml
  label: Prodsmart Suppliers API
  slug: prodsmart-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodsmart/refs/heads/main/openapi/prodsmart-suppliers-api-openapi.yml
- filename: prodsmart-task-durations-api-openapi.yml
  format: yaml
  label: Prodsmart Task Durations API
  slug: prodsmart-task-durations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodsmart/refs/heads/main/openapi/prodsmart-task-durations-api-openapi.yml
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Prodsmart Authentication
name_suffix: Authentication
oauth_flows: []
overview: Prodsmart secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Prodsmart
provider_slug: prodsmart
scheme_count: 2
schemes:
- description: API Key as username, API Secret as password; mints a 2-hour token.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/prodsmart-v1-openapi.yml
  type: http
- description: Token passed as the access_token query parameter on most endpoints.
  in: query
  name: accessToken
  parameter: access_token
  sources:
  - openapi/prodsmart-v1-openapi.yml
  type: apiKey
slug: prodsmart-authentication
source_filename: prodsmart-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://help.fusionoperations.autodesk.com/en/articles/7257724-autodesk-fusion-operations-api\ndocs: https://fusionoperations.autodesk.com/api-documentation\nsummary:\n  types: [http, apiKey]\n  http_schemes: [basic]\n  api_key_in: [query]\n  oauth2_flows: []\n  notes: >-\n    v1 uses HTTP Basic auth (API Key = username, API Secret = password) to mint a\n    bearer token valid for 2 hours; most endpoints also accept the token via an\n    access_token query parameter. API credentials are requested from the company\n    profile (\"Request an API key\"). An API key is mandatory to activate Webhooks,\n    Zapier and Changes Feed Channel integrations. The current v2 API is hosted on\n    Autodesk Platform Services (APS) and follows APS auth.\nschemes:\n  - name: basicAuth\n    type: http\n    scheme: basic\n    description: API Key as username, API Secret as password; mints a 2-hour token.\n    sources: [openapi/prodsmart-v1-openapi.yml]\n\
  \  - name: accessToken\n    type: apiKey\n    in: query\n    parameter: access_token\n    description: Token passed as the access_token query parameter on most endpoints.\n    sources: [openapi/prodsmart-v1-openapi.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prodsmart/refs/heads/main/authentication/prodsmart-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- Company
- Manufacturing
- Manufacturing Execution System
- Production Management
- Inventory
- Shop Floor
- Autodesk
- Industry 4.0
---
