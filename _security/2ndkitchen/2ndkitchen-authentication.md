---
api_key_in: []
api_specs:
- filename: 2ndkitchen-authentication-api-openapi.yml
  format: yaml
  label: 2ndKitchen Authentication API
  slug: 2ndkitchen-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-authentication-api-openapi.yml
- filename: 2ndkitchen-brand-api-openapi.yml
  format: yaml
  label: 2ndKitchen Brand API
  slug: 2ndkitchen-brand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-brand-api-openapi.yml
- filename: 2ndkitchen-business-api-openapi.yml
  format: yaml
  label: 2ndKitchen Business API
  slug: 2ndkitchen-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-business-api-openapi.yml
- filename: 2ndkitchen-coupons-api-openapi.yml
  format: yaml
  label: 2ndKitchen Coupons API
  slug: 2ndkitchen-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-coupons-api-openapi.yml
- filename: 2ndkitchen-deliveries-api-openapi.yml
  format: yaml
  label: 2ndKitchen Deliveries API
  slug: 2ndkitchen-deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-deliveries-api-openapi.yml
- filename: 2ndkitchen-orders-api-openapi.yml
  format: yaml
  label: 2ndKitchen Orders API
  slug: 2ndkitchen-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-orders-api-openapi.yml
- filename: 2ndkitchen-payment-api-openapi.yml
  format: yaml
  label: 2ndKitchen Payment API
  slug: 2ndkitchen-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-payment-api-openapi.yml
- filename: 2ndkitchen-product-api-openapi.yml
  format: yaml
  label: 2ndKitchen Product API
  slug: 2ndkitchen-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-product-api-openapi.yml
- filename: 2ndkitchen-products-api-openapi.yml
  format: yaml
  label: 2ndKitchen Products API
  slug: 2ndkitchen-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-products-api-openapi.yml
- filename: 2ndkitchen-restaurant-api-openapi.yml
  format: yaml
  label: 2ndKitchen Restaurant API
  slug: 2ndkitchen-restaurant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-restaurant-api-openapi.yml
- filename: 2ndkitchen-restaurants-api-openapi.yml
  format: yaml
  label: 2ndKitchen Restaurants API
  slug: 2ndkitchen-restaurants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-restaurants-api-openapi.yml
- filename: 2ndkitchen-users-api-openapi.yml
  format: yaml
  label: 2ndKitchen Users API
  slug: 2ndkitchen-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: 2Ndkitchen Authentication
name_suffix: Authentication
oauth_flows: []
overview: 2ndKitchen secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: 2ndKitchen
provider_slug: 2ndkitchen
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: In order to use Bond API, each request must be authenticated with an API key. The API key should be sent with each request in the header section with the header
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/2ndkitchen-businessservice.yaml
  - openapi/2ndkitchen-paymentservice.yaml
  - openapi/2ndkitchen-restaurantservice.yaml
  - openapi/2ndkitchen-userservice.yaml
  type: http
slug: 2ndkitchen-authentication
source_filename: 2ndkitchen-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: derived\nsource: openapi/2ndkitchen-businessservice.yaml, openapi/2ndkitchen-paymentservice.yaml, openapi/2ndkitchen-restaurantservice.yaml,\n  openapi/2ndkitchen-userservice.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: In order to use Bond API, each request must be authenticated with an API key.\n    The API key should be sent with each request in the header section with the header\n  sources:\n  - openapi/2ndkitchen-businessservice.yaml\n  - openapi/2ndkitchen-paymentservice.yaml\n  - openapi/2ndkitchen-restaurantservice.yaml\n  - openapi/2ndkitchen-userservice.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/authentication/2ndkitchen-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Food Technology
- Ghost Kitchen
- Restaurant
- Food Delivery
- Ordering
- Payments
- Hospitality
- Techstars
- Acquired
---
