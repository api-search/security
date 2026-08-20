---
api_key_in:
- formData
- header
- query
api_specs:
- filename: vinculum-advance-shipping-notice-api-openapi.yml
  format: yaml
  label: Vinculum Advance Shipping Notice API
  slug: vinculum-advance-shipping-notice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinculum/refs/heads/main/openapi/vinculum-advance-shipping-notice-api-openapi.yml
- filename: vinculum-authentication-process-api-openapi.yml
  format: yaml
  label: Vinculum Authentication Process API
  slug: vinculum-authentication-process-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinculum/refs/heads/main/openapi/vinculum-authentication-process-api-openapi.yml
- filename: vinculum-common-api-openapi.yml
  format: yaml
  label: Vinculum Common API
  slug: vinculum-common-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinculum/refs/heads/main/openapi/vinculum-common-api-openapi.yml
- filename: vinculum-courier-allocation-process-api-openapi.yml
  format: yaml
  label: Vinculum Courier Allocation Process API
  slug: vinculum-courier-allocation-process-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinculum/refs/heads/main/openapi/vinculum-courier-allocation-process-api-openapi.yml
- filename: vinculum-inbounds-api-openapi.yml
  format: yaml
  label: Vinculum Inbounds API
  slug: vinculum-inbounds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinculum/refs/heads/main/openapi/vinculum-inbounds-api-openapi.yml
- filename: vinculum-listing-managment-api-openapi.yml
  format: yaml
  label: Vinculum Listing Managment API
  slug: vinculum-listing-managment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinculum/refs/heads/main/openapi/vinculum-listing-managment-api-openapi.yml
- filename: vinculum-manifest-api-openapi.yml
  format: yaml
  label: Vinculum Manifest API
  slug: vinculum-manifest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinculum/refs/heads/main/openapi/vinculum-manifest-api-openapi.yml
- filename: vinculum-order-managment-api-openapi.yml
  format: yaml
  label: Vinculum Order Managment API
  slug: vinculum-order-managment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinculum/refs/heads/main/openapi/vinculum-order-managment-api-openapi.yml
- filename: vinculum-order-returns-api-openapi.yml
  format: yaml
  label: Vinculum Order Returns API
  slug: vinculum-order-returns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinculum/refs/heads/main/openapi/vinculum-order-returns-api-openapi.yml
- filename: vinculum-orders-api-openapi.yml
  format: yaml
  label: Vinculum Orders API
  slug: vinculum-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinculum/refs/heads/main/openapi/vinculum-orders-api-openapi.yml
- filename: vinculum-products-api-openapi.yml
  format: yaml
  label: Vinculum Products API
  slug: vinculum-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinculum/refs/heads/main/openapi/vinculum-products-api-openapi.yml
- filename: vinculum-purchase-orders-api-openapi.yml
  format: yaml
  label: Vinculum Purchase Orders API
  slug: vinculum-purchase-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinculum/refs/heads/main/openapi/vinculum-purchase-orders-api-openapi.yml
- filename: vinculum-putaway-api-openapi.yml
  format: yaml
  label: Vinculum Putaway API
  slug: vinculum-putaway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinculum/refs/heads/main/openapi/vinculum-putaway-api-openapi.yml
- filename: vinculum-return-to-vendor-api-openapi.yml
  format: yaml
  label: Vinculum Return to Vendor API
  slug: vinculum-return-to-vendor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinculum/refs/heads/main/openapi/vinculum-return-to-vendor-api-openapi.yml
- filename: vinculum-stock-api-openapi.yml
  format: yaml
  label: Vinculum Stock API
  slug: vinculum-stock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinculum/refs/heads/main/openapi/vinculum-stock-api-openapi.yml
- filename: vinculum-transfers-api-openapi.yml
  format: yaml
  label: Vinculum Transfers API
  slug: vinculum-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinculum/refs/heads/main/openapi/vinculum-transfers-api-openapi.yml
- filename: vinculum-vendors-api-openapi.yml
  format: yaml
  label: Vinculum Vendors API
  slug: vinculum-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinculum/refs/heads/main/openapi/vinculum-vendors-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Vinculum Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vinculum secures its APIs with apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Vinculum
provider_slug: vinculum
scheme_count: 4
schemes:
- description: Client/account identifier issued by Vinculum, paired with ApiKey.
  in:
  - formData
  - header
  - query
  name: ApiOwner
  parameter: ApiOwner
  sources:
  - openapi/vinculum-eretail-openapi-original.yml
  type: apiKey
- description: Secret key issued by Vinculum, paired with ApiOwner on every eRetail call.
  in:
  - formData
  - header
  - query
  name: ApiKey
  parameter: ApiKey
  sources:
  - openapi/vinculum-eretail-openapi-original.yml
  type: apiKey
- description: Tenant database selector header used on multi-tenant deployments.
  in:
  - header
  name: DbId
  parameter: DbId
  sources:
  - openapi/vinculum-eretail-openapi-original.yml
  type: apiKey
- description: SellerPanel V3 exchanges username + password (query params) at /authToken for a token presented on subsequent SellerPanel operations.
  flow: username-password
  name: SellerPanelToken
  sources:
  - openapi/vinculum-sellerpanel-openapi-original.yml
  token_endpoint: GET /RestWS/api/sellerPanel/v3/authToken
  type: token
slug: vinculum-authentication
source_filename: vinculum-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://erp.vineretail.com/swagger/ + https://erp.vineretail.com/SellerPanelV3/\ndocs: https://docs.vineretail.com\nsummary:\n  types: [apiKey]\n  api_key_in: [formData, header, query]\n  oauth2_flows: []\n  notes: >-\n    Vin eRetail authenticates every request with a paired ApiOwner + ApiKey\n    credential (issued per client/warehouse). The credential is accepted in\n    form-data, HTTP header, or query string depending on the operation. A DbId /\n    DBID header selects the tenant database on some operations. The SellerPanel\n    V3 API instead exchanges a username + password at GET /authToken for a\n    session token used on subsequent calls. Neither API declares a formal\n    OpenAPI securityScheme; the credentials are modeled as operation parameters.\nschemes:\n  - name: ApiOwner\n    type: apiKey\n    in: [formData, header, query]\n    parameter: ApiOwner\n    description: Client/account identifier issued by Vinculum,\
  \ paired with ApiKey.\n    sources: [openapi/vinculum-eretail-openapi-original.yml]\n  - name: ApiKey\n    type: apiKey\n    in: [formData, header, query]\n    parameter: ApiKey\n    description: Secret key issued by Vinculum, paired with ApiOwner on every eRetail call.\n    sources: [openapi/vinculum-eretail-openapi-original.yml]\n  - name: DbId\n    type: apiKey\n    in: [header]\n    parameter: DbId\n    description: Tenant database selector header used on multi-tenant deployments.\n    sources: [openapi/vinculum-eretail-openapi-original.yml]\n  - name: SellerPanelToken\n    type: token\n    flow: username-password\n    token_endpoint: GET /RestWS/api/sellerPanel/v3/authToken\n    description: >-\n      SellerPanel V3 exchanges username + password (query params) at /authToken\n      for a token presented on subsequent SellerPanel operations.\n    sources: [openapi/vinculum-sellerpanel-openapi-original.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vinculum/refs/heads/main/authentication/vinculum-authentication.yml
summary_line: apiKey · 4 schemes
tags:
- Company
- E-Commerce
- Omnichannel
- Order Management
- Warehouse Management
- Inventory
- Retail
- Marketplaces
---
