---
api_key_in:
- formData
- header
- query
api_specs:
- filename: vinculum-eretail-openapi-original.yml
  format: yaml
  label: Vin eRetail API
  slug: vin-eretail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinculum/refs/heads/main/openapi/vinculum-eretail-openapi-original.yml
- filename: vinculum-sellerpanel-openapi-original.yml
  format: yaml
  label: Vin eRetail SellerPanel V3 API
  slug: vin-eretail-sellerpanel-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinculum/refs/heads/main/openapi/vinculum-sellerpanel-openapi-original.yml
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
- Ecommerce
- Omnichannel
- Order Management
- Warehouse Management
- Inventory
- Retail
- Marketplaces
---
