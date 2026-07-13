---
api_key_in: []
api_specs:
- filename: sendle-orders-api-openapi.yml
  format: yaml
  label: Sendle Orders API
  slug: sendle-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendle/refs/heads/main/openapi/sendle-orders-api-openapi.yml
- filename: sendle-products-api-openapi.yml
  format: yaml
  label: Sendle Products & Quoting API
  slug: sendle-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendle/refs/heads/main/openapi/sendle-products-api-openapi.yml
- filename: sendle-tracking-api-openapi.yml
  format: yaml
  label: Sendle Tracking API
  slug: sendle-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendle/refs/heads/main/openapi/sendle-tracking-api-openapi.yml
- filename: sendle-manifests-api-openapi.yml
  format: yaml
  label: Sendle Shipping Manifests API
  slug: sendle-manifests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendle/refs/heads/main/openapi/sendle-manifests-api-openapi.yml
- filename: sendle-ping-api-openapi.yml
  format: yaml
  label: Sendle Ping API
  slug: sendle-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendle/refs/heads/main/openapi/sendle-ping-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sendle Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sendle secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sendle
provider_slug: sendle
scheme_count: 1
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/sendle-manifests-api-openapi.yml
  - openapi/sendle-orders-api-openapi.yml
  - openapi/sendle-ping-api-openapi.yml
  - openapi/sendle-products-api-openapi.yml
  - openapi/sendle-tracking-api-openapi.yml
  type: http
slug: sendle-authentication
source_filename: sendle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sendle-manifests-api-openapi.yml, openapi/sendle-orders-api-openapi.yml, openapi/sendle-ping-api-openapi.yml,\n  openapi/sendle-products-api-openapi.yml, openapi/sendle-tracking-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/sendle-manifests-api-openapi.yml\n  - openapi/sendle-orders-api-openapi.yml\n  - openapi/sendle-ping-api-openapi.yml\n  - openapi/sendle-products-api-openapi.yml\n  - openapi/sendle-tracking-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sendle/refs/heads/main/authentication/sendle-authentication.yml
summary_line: http · 1 scheme
tags:
- Shipping
- Logistics
- Last Mile
- Parcels
- E-commerce
- Carbon Neutral
- Small Business
- Australia
- United States
- Canada
---
