---
api_key_in:
- header
api_specs:
- filename: prodigi-openapi.yml
  format: yaml
  label: Prodigi Orders API
  slug: prodigi-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodigi/refs/heads/main/openapi/prodigi-openapi.yml
- filename: prodigi-openapi.yml
  format: yaml
  label: Prodigi Quotes API
  slug: prodigi-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodigi/refs/heads/main/openapi/prodigi-openapi.yml
- filename: prodigi-openapi.yml
  format: yaml
  label: Prodigi Product Details API
  slug: prodigi-product-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodigi/refs/heads/main/openapi/prodigi-openapi.yml
- filename: prodigi-openapi.yml
  format: yaml
  label: Prodigi Webhooks / Callbacks
  slug: prodigi-webhooks-callbacks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodigi/refs/heads/main/openapi/prodigi-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Prodigi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Prodigi secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Prodigi
provider_slug: prodigi
scheme_count: 1
schemes:
- description: Your Prodigi API key, sent in the X-API-Key header on every request.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/prodigi-openapi.yml
  type: apiKey
slug: prodigi-authentication
source_filename: prodigi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/prodigi-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Your Prodigi API key, sent in the X-API-Key header on every request.\n  sources:\n  - openapi/prodigi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prodigi/refs/heads/main/authentication/prodigi-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Print on Demand
- Printing
- Dropshipping
- Fulfillment
- E-commerce
---
