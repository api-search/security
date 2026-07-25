---
api_key_in: []
api_specs:
- filename: 99-minutos-coverage-api-openapi.yml
  format: yaml
  label: 99 Minutos coverage API
  slug: 99-minutos-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/99-minutos/refs/heads/main/openapi/99-minutos-coverage-api-openapi.yml
- filename: 99-minutos-documents-api-openapi.yml
  format: yaml
  label: 99 Minutos documents API
  slug: 99-minutos-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/99-minutos/refs/heads/main/openapi/99-minutos-documents-api-openapi.yml
- filename: 99-minutos-locations-api-openapi.yml
  format: yaml
  label: 99 Minutos locations API
  slug: 99-minutos-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/99-minutos/refs/heads/main/openapi/99-minutos-locations-api-openapi.yml
- filename: 99-minutos-oauth-api-openapi.yml
  format: yaml
  label: 99 Minutos oauth API
  slug: 99-minutos-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/99-minutos/refs/heads/main/openapi/99-minutos-oauth-api-openapi.yml
- filename: 99-minutos-orders-api-openapi.yml
  format: yaml
  label: 99 Minutos Orders API
  slug: 99-minutos-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/99-minutos/refs/heads/main/openapi/99-minutos-orders-api-openapi.yml
- filename: 99-minutos-shipments-api-openapi.yml
  format: yaml
  label: 99 Minutos shipments API
  slug: 99-minutos-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/99-minutos/refs/heads/main/openapi/99-minutos-shipments-api-openapi.yml
- filename: 99-minutos-shipping-rates-api-openapi.yml
  format: yaml
  label: 99 Minutos shipping-rates API
  slug: 99-minutos-shipping-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/99-minutos/refs/heads/main/openapi/99-minutos-shipping-rates-api-openapi.yml
- filename: 99-minutos-super-geocoding-api-openapi.yml
  format: yaml
  label: 99 Minutos super-geocoding API
  slug: 99-minutos-super-geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/99-minutos/refs/heads/main/openapi/99-minutos-super-geocoding-api-openapi.yml
- filename: 99-minutos-webhooks-api-openapi.yml
  format: yaml
  label: 99 Minutos webhooks API
  slug: 99-minutos-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/99-minutos/refs/heads/main/openapi/99-minutos-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: 99 Minutos Authentication
name_suffix: Authentication
oauth_flows: []
overview: 99 Minutos secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: 99 Minutos
provider_slug: 99-minutos
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: AuthJWT
  scheme: bearer
  sources:
  - openapi/99minutos-api-v3-openapi.json
  type: http
slug: 99-minutos-authentication
source_filename: 99-minutos-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: derived\nsource: openapi/99minutos-api-v3-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: AuthJWT\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/99minutos-api-v3-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/99-minutos/refs/heads/main/authentication/99-minutos-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Logistics
- Last Mile Delivery
- Shipping
- Ecommerce
- Fulfillment
- Freight
- Tracking
- Webhooks
- Latin America
- Mexico
---
