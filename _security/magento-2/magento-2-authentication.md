---
api_key_in: []
api_specs:
- filename: magento-2-auth-api-openapi.yml
  format: yaml
  label: Magento 2 (Adobe Commerce) Auth API
  slug: magento-2-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magento-2/refs/heads/main/openapi/magento-2-auth-api-openapi.yml
- filename: magento-2-carts-api-openapi.yml
  format: yaml
  label: Magento 2 (Adobe Commerce) Carts API
  slug: magento-2-carts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magento-2/refs/heads/main/openapi/magento-2-carts-api-openapi.yml
- filename: magento-2-categories-api-openapi.yml
  format: yaml
  label: Magento 2 (Adobe Commerce) Categories API
  slug: magento-2-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magento-2/refs/heads/main/openapi/magento-2-categories-api-openapi.yml
- filename: magento-2-customers-api-openapi.yml
  format: yaml
  label: Magento 2 (Adobe Commerce) Customers API
  slug: magento-2-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magento-2/refs/heads/main/openapi/magento-2-customers-api-openapi.yml
- filename: magento-2-orders-api-openapi.yml
  format: yaml
  label: Magento 2 (Adobe Commerce) Orders API
  slug: magento-2-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magento-2/refs/heads/main/openapi/magento-2-orders-api-openapi.yml
- filename: magento-2-products-api-openapi.yml
  format: yaml
  label: Magento 2 (Adobe Commerce) Products API
  slug: magento-2-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magento-2/refs/heads/main/openapi/magento-2-products-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Magento 2 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Magento 2 (Adobe Commerce) secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Magento 2 (Adobe Commerce)
provider_slug: magento-2
scheme_count: 1
schemes:
- description: Bearer token obtained from /V1/integration/admin/token or /V1/integration/customer/token.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/magento-2-openapi.yml
  type: http
slug: magento-2-authentication
source_filename: magento-2-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/magento-2-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token obtained from /V1/integration/admin/token or /V1/integration/customer/token.\n  sources:\n  - openapi/magento-2-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/magento-2/refs/heads/main/authentication/magento-2-authentication.yml
summary_line: http · 1 scheme
tags:
- Ecommerce
- Commerce
- Online Store
- Catalog Management
- Order Management
- GraphQL
- REST
- SOAP
---
