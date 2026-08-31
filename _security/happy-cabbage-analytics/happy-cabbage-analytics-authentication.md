---
api_key_in:
- header
api_specs:
- filename: happy-cabbage-analytics-blockout-dates-api-openapi.yml
  format: yaml
  label: Happy Cabbage Analytics Blockout Dates API
  slug: happy-cabbage-analytics-blockout-dates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happy-cabbage-analytics/refs/heads/main/openapi/happy-cabbage-analytics-blockout-dates-api-openapi.yml
- filename: happy-cabbage-analytics-daily-sales-metadata-api-openapi.yml
  format: yaml
  label: Happy Cabbage Analytics Daily Sales Metadata API
  slug: happy-cabbage-analytics-daily-sales-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happy-cabbage-analytics/refs/heads/main/openapi/happy-cabbage-analytics-daily-sales-metadata-api-openapi.yml
- filename: happy-cabbage-analytics-identity-api-openapi.yml
  format: yaml
  label: Happy Cabbage Analytics Identity API
  slug: happy-cabbage-analytics-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happy-cabbage-analytics/refs/heads/main/openapi/happy-cabbage-analytics-identity-api-openapi.yml
- filename: happy-cabbage-analytics-inventory-health-api-openapi.yml
  format: yaml
  label: Happy Cabbage Analytics Inventory Health API
  slug: happy-cabbage-analytics-inventory-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happy-cabbage-analytics/refs/heads/main/openapi/happy-cabbage-analytics-inventory-health-api-openapi.yml
- filename: happy-cabbage-analytics-orders-api-openapi.yml
  format: yaml
  label: Happy Cabbage Analytics Orders API
  slug: happy-cabbage-analytics-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happy-cabbage-analytics/refs/heads/main/openapi/happy-cabbage-analytics-orders-api-openapi.yml
- filename: happy-cabbage-analytics-packages-api-openapi.yml
  format: yaml
  label: Happy Cabbage Analytics Packages API
  slug: happy-cabbage-analytics-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happy-cabbage-analytics/refs/heads/main/openapi/happy-cabbage-analytics-packages-api-openapi.yml
- filename: happy-cabbage-analytics-pos-brands-api-openapi.yml
  format: yaml
  label: Happy Cabbage Analytics POS Brands API
  slug: happy-cabbage-analytics-pos-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happy-cabbage-analytics/refs/heads/main/openapi/happy-cabbage-analytics-pos-brands-api-openapi.yml
- filename: happy-cabbage-analytics-pos-categories-api-openapi.yml
  format: yaml
  label: Happy Cabbage Analytics POS Categories API
  slug: happy-cabbage-analytics-pos-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happy-cabbage-analytics/refs/heads/main/openapi/happy-cabbage-analytics-pos-categories-api-openapi.yml
- filename: happy-cabbage-analytics-product-inventory-api-openapi.yml
  format: yaml
  label: Happy Cabbage Analytics Product Inventory API
  slug: happy-cabbage-analytics-product-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happy-cabbage-analytics/refs/heads/main/openapi/happy-cabbage-analytics-product-inventory-api-openapi.yml
- filename: happy-cabbage-analytics-product-line-inventory-api-openapi.yml
  format: yaml
  label: Happy Cabbage Analytics Product Line Inventory API
  slug: happy-cabbage-analytics-product-line-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happy-cabbage-analytics/refs/heads/main/openapi/happy-cabbage-analytics-product-line-inventory-api-openapi.yml
- filename: happy-cabbage-analytics-product-lines-api-openapi.yml
  format: yaml
  label: Happy Cabbage Analytics Product Lines API
  slug: happy-cabbage-analytics-product-lines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happy-cabbage-analytics/refs/heads/main/openapi/happy-cabbage-analytics-product-lines-api-openapi.yml
- filename: happy-cabbage-analytics-stores-api-openapi.yml
  format: yaml
  label: Happy Cabbage Analytics Stores API
  slug: happy-cabbage-analytics-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happy-cabbage-analytics/refs/heads/main/openapi/happy-cabbage-analytics-stores-api-openapi.yml
- filename: happy-cabbage-analytics-universal-brands-api-openapi.yml
  format: yaml
  label: Happy Cabbage Analytics Universal Brands API
  slug: happy-cabbage-analytics-universal-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happy-cabbage-analytics/refs/heads/main/openapi/happy-cabbage-analytics-universal-brands-api-openapi.yml
- filename: happy-cabbage-analytics-universal-categories-api-openapi.yml
  format: yaml
  label: Happy Cabbage Analytics Universal Categories API
  slug: happy-cabbage-analytics-universal-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happy-cabbage-analytics/refs/heads/main/openapi/happy-cabbage-analytics-universal-categories-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Happy Cabbage Analytics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Happy Cabbage Analytics secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Happy Cabbage Analytics
provider_slug: happy-cabbage-analytics
scheme_count: 1
schemes:
- description: External API key issued by Happy Buyers. Send the key in the hca-api-key header.
  in: header
  name: ApiKeyAuth
  parameter: hca-api-key
  sources:
  - openapi/happy-cabbage-analytics-happy-buyers-external-openapi.yml
  type: apiKey
slug: happy-cabbage-analytics-authentication
source_filename: happy-cabbage-analytics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: derived\nsource: openapi/happy-cabbage-analytics-happy-buyers-external-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: hca-api-key\n  description: External API key issued by Happy Buyers. Send the key in the hca-api-key header.\n  sources:\n  - openapi/happy-cabbage-analytics-happy-buyers-external-openapi.yml\ndocs: https://cabbage.pub/swagger-ui/index.html\nnote: 'Single scheme. The Happy Buyers External API is API-key only: no OAuth, no OIDC, no mTLS, no bearer tokens.\n  Keys are issued by Happy Buyers per organization and every response is scoped to that organization, so the key\n  IS the tenant selector — there is no account/tenant parameter anywhere in the contract. GET /external/v1/whoami\n  is the documented way to resolve which key and organization you are operating as. Happy Cabbage publishes no prose\n  authentication page; the Swagger\
  \ UI at cabbage.pub is the whole developer surface.'\ntenancy:\n  model: key-scoped organization\n  resolver_operation: whoami\n  resolver_path: /external/v1/whoami\n  returns:\n  - keyName\n  - organizationName\n  - keyCreatedAt\n  - organizationCreatedAt\nkey_scopes:\n  model: per-key permissions\n  declared_in: 403 response descriptions on individual operations only — there is no securityScheme scope list,\n    no scopes reference page and no scope introspection endpoint\n  values:\n  - scope: organization_metadata:read\n    operations:\n    - getStores\n    - getPosBrands\n    - getPosCategories\n    - getUniversalBrands\n  - scope: inventory:read\n    operations:\n    - getProductInventory\n    - getProductLineInventory\n    - findPackages\n    - getStoreInventoryHealths\n    - getStoreInventoryHealthHistories\n    - getPosBrandInventoryHealths\n    - getPosBrandInventoryHealthHistory\n    - getCategoryInventoryHealths\n    - getCategoryInventoryHealthHistories\n    - getDailySalesMetadataForProduct\n\
  \  - scope: inventory:write\n    operations:\n    - updateCarryStatus\n  - scope: product_lines:read\n    operations:\n    - getProductLines\n    - getProductLine\n  - scope: product_lines:write\n    operations:\n    - createProductLine\n    - updateProductLine\n  - scope: orders:write\n    operations:\n    - createOrder\n    - updateOrder\n  note: These are API-key permissions, not OAuth scopes, so no scopes/ artifact with an OAuthScopes pointer is emitted.\n    Nineteen of the 40 operations declare no 403 at all — chiefly the order-item, order-invoice, blockout-date and\n    whoami operations — so their scope requirement is undocumented.\nunauthenticated_behaviour:\n  method: probed\n  source: https://api.happycabbage.ai/external/v1/whoami\n  status: 403\n  body: '{\"timestamp\":\"...\",\"status\":403,\"error\":\"Forbidden\",\"path\":\"/...\"}'\n  note: The gateway returns 403 rather than the contract-declared 401 for a wholly absent key, and the body is the\n    Spring Boot default\
  \ envelope with no WWW-Authenticate header.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/happy-cabbage-analytics/refs/heads/main/authentication/happy-cabbage-analytics-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cannabis
- Retail
- Inventory Management
- Analytics
- Purchasing
- Point of Sale
- Wholesale
- Demand Forecasting
- Supply Chain
- agent-native
---
