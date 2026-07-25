---
api_key_in:
- header
api_specs:
- filename: stamped-customer-actions-api-openapi.yml
  format: yaml
  label: Stamped Customer Actions API
  slug: stamped-customer-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stamped/refs/heads/main/openapi/stamped-customer-actions-api-openapi.yml
- filename: stamped-customers-api-openapi.yml
  format: yaml
  label: Stamped Customers API
  slug: stamped-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stamped/refs/heads/main/openapi/stamped-customers-api-openapi.yml
- filename: stamped-orders-api-openapi.yml
  format: yaml
  label: Stamped Orders API
  slug: stamped-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stamped/refs/heads/main/openapi/stamped-orders-api-openapi.yml
- filename: stamped-products-api-openapi.yml
  format: yaml
  label: Stamped Products API
  slug: stamped-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stamped/refs/heads/main/openapi/stamped-products-api-openapi.yml
- filename: stamped-program-reporting-api-openapi.yml
  format: yaml
  label: Stamped Program Reporting API
  slug: stamped-program-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stamped/refs/heads/main/openapi/stamped-program-reporting-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Stamped Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stamped secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Stamped
provider_slug: stamped
scheme_count: 1
schemes:
- in: header
  name: StampedApiKeyAuth
  parameter: stamped-api-key
  sources:
  - openapi/stamped-loyalty-operations-openapi.json
  - openapi/stamped-merchant-data-openapi.json
  type: apiKey
slug: stamped-authentication
source_filename: stamped-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/stamped-loyalty-operations-openapi.json, openapi/stamped-merchant-data-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: StampedApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: stamped-api-key\n  sources:\n  - openapi/stamped-loyalty-operations-openapi.json\n  - openapi/stamped-merchant-data-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stamped/refs/heads/main/authentication/stamped-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Consumer
- Reviews
- Ratings
- Loyalty
- E-Commerce
- Customer Marketing
- Shopify
---
