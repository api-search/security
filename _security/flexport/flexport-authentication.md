---
api_key_in: []
api_specs:
- filename: flexport-bookings-api-openapi.yml
  format: yaml
  label: Flexport Bookings API
  slug: flexport-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexport/refs/heads/main/openapi/flexport-bookings-api-openapi.yml
- filename: flexport-customs-api-openapi.yml
  format: yaml
  label: Flexport Customs API
  slug: flexport-customs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexport/refs/heads/main/openapi/flexport-customs-api-openapi.yml
- filename: flexport-documents-api-openapi.yml
  format: yaml
  label: Flexport Documents API
  slug: flexport-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexport/refs/heads/main/openapi/flexport-documents-api-openapi.yml
- filename: flexport-invoices-api-openapi.yml
  format: yaml
  label: Flexport Invoices API
  slug: flexport-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexport/refs/heads/main/openapi/flexport-invoices-api-openapi.yml
- filename: flexport-network-api-openapi.yml
  format: yaml
  label: Flexport Network API
  slug: flexport-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexport/refs/heads/main/openapi/flexport-network-api-openapi.yml
- filename: flexport-products-api-openapi.yml
  format: yaml
  label: Flexport Products API
  slug: flexport-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexport/refs/heads/main/openapi/flexport-products-api-openapi.yml
- filename: flexport-purchaseorders-api-openapi.yml
  format: yaml
  label: Flexport PurchaseOrders API
  slug: flexport-purchaseorders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexport/refs/heads/main/openapi/flexport-purchaseorders-api-openapi.yml
- filename: flexport-shipments-api-openapi.yml
  format: yaml
  label: Flexport Shipments API
  slug: flexport-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexport/refs/heads/main/openapi/flexport-shipments-api-openapi.yml
- filename: flexport-webhooks-api-openapi.yml
  format: yaml
  label: Flexport Webhooks API
  slug: flexport-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexport/refs/heads/main/openapi/flexport-webhooks-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Flexport Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Flexport secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Flexport
provider_slug: flexport
scheme_count: 2
schemes:
- description: OAuth 2.0 client credentials issued from the Flexport admin console
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.flexport.com/oauth/token
  name: oauth2
  sources:
  - openapi/flexport-openapi.yml
  type: oauth2
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/flexport-openapi.yml
  type: http
slug: flexport-authentication
source_filename: flexport-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/flexport-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.flexport.com/oauth/token\n    scopes: 0\n  description: OAuth 2.0 client credentials issued from the Flexport admin console\n  sources:\n  - openapi/flexport-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/flexport-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flexport/refs/heads/main/authentication/flexport-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Logistics
- Freight
- Supply Chain
- Customs
- B2B
---
