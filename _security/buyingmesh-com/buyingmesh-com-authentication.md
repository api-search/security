---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: buyingmesh-com-admin-api-openapi.yml
  format: yaml
  label: BuyingMesh Admin API
  slug: buyingmesh-com-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyingmesh-com/openapi/buyingmesh-com-admin-api-openapi.yml
- filename: buyingmesh-com-buyer-confirmations-api-openapi.yml
  format: yaml
  label: BuyingMesh Buyer Confirmations API
  slug: buyingmesh-com-buyer-confirmations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyingmesh-com/openapi/buyingmesh-com-buyer-confirmations-api-openapi.yml
- filename: buyingmesh-com-inquiries-api-openapi.yml
  format: yaml
  label: BuyingMesh Inquiries API
  slug: buyingmesh-com-inquiries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyingmesh-com/openapi/buyingmesh-com-inquiries-api-openapi.yml
- filename: buyingmesh-com-landed-cost-api-openapi.yml
  format: yaml
  label: BuyingMesh Landed Cost API
  slug: buyingmesh-com-landed-cost-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyingmesh-com/openapi/buyingmesh-com-landed-cost-api-openapi.yml
- filename: buyingmesh-com-merchant-api-openapi.yml
  format: yaml
  label: BuyingMesh Merchant API
  slug: buyingmesh-com-merchant-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyingmesh-com/openapi/buyingmesh-com-merchant-api-openapi.yml
- filename: buyingmesh-com-orders-api-openapi.yml
  format: yaml
  label: BuyingMesh Orders API
  slug: buyingmesh-com-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyingmesh-com/openapi/buyingmesh-com-orders-api-openapi.yml
- filename: buyingmesh-com-products-api-openapi.yml
  format: yaml
  label: BuyingMesh Products API
  slug: buyingmesh-com-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyingmesh-com/openapi/buyingmesh-com-products-api-openapi.yml
- filename: buyingmesh-com-quotes-api-openapi.yml
  format: yaml
  label: BuyingMesh Quotes API
  slug: buyingmesh-com-quotes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyingmesh-com/openapi/buyingmesh-com-quotes-api-openapi.yml
- filename: buyingmesh-com-shipping-api-openapi.yml
  format: yaml
  label: BuyingMesh Shipping API
  slug: buyingmesh-com-shipping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyingmesh-com/openapi/buyingmesh-com-shipping-api-openapi.yml
- filename: buyingmesh-com-suppliers-api-openapi.yml
  format: yaml
  label: BuyingMesh Suppliers API
  slug: buyingmesh-com-suppliers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyingmesh-com/openapi/buyingmesh-com-suppliers-api-openapi.yml
- filename: buyingmesh-com-support-api-openapi.yml
  format: yaml
  label: BuyingMesh Support API
  slug: buyingmesh-com-support-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyingmesh-com/openapi/buyingmesh-com-support-api-openapi.yml
- filename: buyingmesh-com-tariffs-api-openapi.yml
  format: yaml
  label: BuyingMesh Tariffs API
  slug: buyingmesh-com-tariffs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyingmesh-com/openapi/buyingmesh-com-tariffs-api-openapi.yml
- filename: buyingmesh-com-webhook-deliveries-api-openapi.yml
  format: yaml
  label: BuyingMesh Webhook Deliveries API
  slug: buyingmesh-com-webhook-deliveries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyingmesh-com/openapi/buyingmesh-com-webhook-deliveries-api-openapi.yml
- filename: buyingmesh-com-webhook-subscriptions-api-openapi.yml
  format: yaml
  label: BuyingMesh Webhook Subscriptions API
  slug: buyingmesh-com-webhook-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyingmesh-com/openapi/buyingmesh-com-webhook-subscriptions-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Buyingmesh Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: BuyingMesh secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: BuyingMesh
provider_slug: buyingmesh-com
scheme_count: 2
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/buyingmesh-com-openapi.yaml
  type: http
- in: header
  name: adminReviewKey
  parameter: X-Admin-Key
  sources:
  - openapi/buyingmesh-com-openapi.yaml
  type: apiKey
slug: buyingmesh-com-authentication
source_filename: buyingmesh-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: derived\nsource: openapi/buyingmesh-com-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/buyingmesh-com-openapi.yaml\n- name: adminReviewKey\n  type: apiKey\n  in: header\n  parameter: X-Admin-Key\n  sources:\n  - openapi/buyingmesh-com-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/buyingmesh-com/authentication/buyingmesh-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Procurement
- Artificial Intelligence
- Catalog
- B2B
- Marketplace
---
