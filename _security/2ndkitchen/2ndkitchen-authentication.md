---
api_key_in: []
api_specs:
- filename: 2ndkitchen-authservice.yaml
  format: yaml
  label: 2ndKitchen Authentication Service
  slug: 2ndkitchen-authentication-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-authservice.yaml
- filename: 2ndkitchen-businessservice.yaml
  format: yaml
  label: 2ndKitchen Business Service
  slug: 2ndkitchen-business-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-businessservice.yaml
- filename: 2ndkitchen-userservice.yaml
  format: yaml
  label: 2ndKitchen User Service
  slug: 2ndkitchen-user-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-userservice.yaml
- filename: 2ndkitchen-restaurantservice.yaml
  format: yaml
  label: 2ndKitchen Restaurant Service
  slug: 2ndkitchen-restaurant-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-restaurantservice.yaml
- filename: 2ndkitchen-orderservice.yaml
  format: yaml
  label: 2ndKitchen Order Service
  slug: 2ndkitchen-order-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-orderservice.yaml
- filename: 2ndkitchen-pricingservice.yaml
  format: yaml
  label: 2ndKitchen Pricing Service
  slug: 2ndkitchen-pricing-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-pricingservice.yaml
- filename: 2ndkitchen-paymentservice.yaml
  format: yaml
  label: 2ndKitchen Payment Service
  slug: 2ndkitchen-payment-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-paymentservice.yaml
- filename: 2ndkitchen-deliveryservice.yaml
  format: yaml
  label: 2ndKitchen Delivery Service
  slug: 2ndkitchen-delivery-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-deliveryservice.yaml
- filename: 2ndkitchen-indexingservice.yaml
  format: yaml
  label: 2ndKitchen Indexing Service
  slug: 2ndkitchen-indexing-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-indexingservice.yaml
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
