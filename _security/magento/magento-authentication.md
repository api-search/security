---
api_key_in: []
api_specs:
- filename: magento-webhooks-asyncapi.yml
  format: yaml
  label: Adobe Commerce Webhooks
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/magento/refs/heads/main/asyncapi/magento-webhooks-asyncapi.yml
- filename: magento-events-asyncapi.yml
  format: yaml
  label: Adobe Commerce Eventing
  slug: events
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/magento/refs/heads/main/asyncapi/magento-events-asyncapi.yml
- filename: magento-authentication-api-openapi.yml
  format: yaml
  label: magento Authentication API
  slug: magento-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magento/refs/heads/main/openapi/magento-authentication-api-openapi.yml
- filename: magento-carts-api-openapi.yml
  format: yaml
  label: magento Carts API
  slug: magento-carts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magento/refs/heads/main/openapi/magento-carts-api-openapi.yml
- filename: magento-categories-api-openapi.yml
  format: yaml
  label: magento Categories API
  slug: magento-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magento/refs/heads/main/openapi/magento-categories-api-openapi.yml
- filename: magento-customers-api-openapi.yml
  format: yaml
  label: magento Customers API
  slug: magento-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magento/refs/heads/main/openapi/magento-customers-api-openapi.yml
- filename: magento-inventory-api-openapi.yml
  format: yaml
  label: magento Inventory API
  slug: magento-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magento/refs/heads/main/openapi/magento-inventory-api-openapi.yml
- filename: magento-invoices-api-openapi.yml
  format: yaml
  label: magento Invoices API
  slug: magento-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magento/refs/heads/main/openapi/magento-invoices-api-openapi.yml
- filename: magento-orders-api-openapi.yml
  format: yaml
  label: magento Orders API
  slug: magento-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magento/refs/heads/main/openapi/magento-orders-api-openapi.yml
- filename: magento-products-api-openapi.yml
  format: yaml
  label: magento Products API
  slug: magento-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magento/refs/heads/main/openapi/magento-products-api-openapi.yml
- filename: magento-shipments-api-openapi.yml
  format: yaml
  label: magento Shipments API
  slug: magento-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magento/refs/heads/main/openapi/magento-shipments-api-openapi.yml
- filename: magento-stores-api-openapi.yml
  format: yaml
  label: magento Stores API
  slug: magento-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magento/refs/heads/main/openapi/magento-stores-api-openapi.yml
- filename: magento-tax-api-openapi.yml
  format: yaml
  label: magento Tax API
  slug: magento-tax-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magento/refs/heads/main/openapi/magento-tax-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Magento Authentication
name_suffix: Authentication
oauth_flows: []
overview: Magento secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Magento
provider_slug: magento
scheme_count: 1
schemes:
- description: Bearer token obtained from the /V1/integration/admin/token or /V1/integration/customer/token endpoint. Include in the Authorization header as "Bearer {token}".
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/magento-rest-api-openapi.yml
  type: http
slug: magento-authentication
source_filename: magento-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/magento-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token obtained from the /V1/integration/admin/token or /V1/integration/customer/token\n    endpoint. Include in the Authorization header as \"Bearer {token}\".\n  sources:\n  - openapi/magento-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/magento/refs/heads/main/authentication/magento-authentication.yml
summary_line: http · 1 scheme
tags: []
---
