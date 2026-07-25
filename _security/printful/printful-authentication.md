---
api_key_in: []
api_specs:
- filename: printful-catalog-api-openapi.yml
  format: yaml
  label: Printful Catalog API
  slug: printful-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printful/refs/heads/main/openapi/printful-catalog-api-openapi.yml
- filename: printful-files-api-openapi.yml
  format: yaml
  label: Printful Files API
  slug: printful-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printful/refs/heads/main/openapi/printful-files-api-openapi.yml
- filename: printful-mockup-generator-api-openapi.yml
  format: yaml
  label: Printful Mockup Generator API
  slug: printful-mockup-generator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printful/refs/heads/main/openapi/printful-mockup-generator-api-openapi.yml
- filename: printful-orders-api-openapi.yml
  format: yaml
  label: Printful Orders API
  slug: printful-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printful/refs/heads/main/openapi/printful-orders-api-openapi.yml
- filename: printful-shipping-rates-api-openapi.yml
  format: yaml
  label: Printful Shipping Rates API
  slug: printful-shipping-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printful/refs/heads/main/openapi/printful-shipping-rates-api-openapi.yml
- filename: printful-store-products-api-openapi.yml
  format: yaml
  label: Printful Store Products API
  slug: printful-store-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printful/refs/heads/main/openapi/printful-store-products-api-openapi.yml
- filename: printful-warehouse-api-openapi.yml
  format: yaml
  label: Printful Warehouse API
  slug: printful-warehouse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printful/refs/heads/main/openapi/printful-warehouse-api-openapi.yml
- filename: printful-webhooks-api-openapi.yml
  format: yaml
  label: Printful Webhooks API
  slug: printful-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printful/refs/heads/main/openapi/printful-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Printful Authentication
name_suffix: Authentication
oauth_flows: []
overview: Printful secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Printful
provider_slug: printful
scheme_count: 1
schemes:
- description: OAuth 2.0 access token or private token passed as a Bearer token in the Authorization header. Account-level tokens must also pass the target store via the X-PF-Store-Id header.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/printful-openapi.yml
  type: http
slug: printful-authentication
source_filename: printful-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/printful-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 access token or private token passed as a Bearer token in the Authorization\n    header. Account-level tokens must also pass the target store via the X-PF-Store-Id header.\n  sources:\n  - openapi/printful-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/printful/refs/heads/main/authentication/printful-authentication.yml
summary_line: http · 1 scheme
tags:
- Print on Demand
- Fulfillment
- Ecommerce
- Dropshipping
- Merchandise
---
