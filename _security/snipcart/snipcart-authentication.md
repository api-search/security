---
api_key_in: []
api_specs:
- filename: snipcart-rest-api-openapi.yml
  format: yaml
  label: Snipcart REST API
  slug: snipcart-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snipcart/refs/heads/main/openapi/snipcart-rest-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Snipcart Authentication
name_suffix: Authentication
oauth_flows: []
overview: Snipcart secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Snipcart
provider_slug: snipcart
scheme_count: 1
schemes:
- description: 'Use your secret API key as the username with an empty password. Base64-encode as {API_KEY}: and pass as Authorization: Basic {encoded}.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/snipcart-rest-api-openapi.yml
  type: http
slug: snipcart-authentication
source_filename: snipcart-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/snipcart-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: 'Use your secret API key as the username with an empty password. Base64-encode\n    as {API_KEY}: and pass as Authorization: Basic {encoded}.'\n  sources:\n  - openapi/snipcart-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snipcart/refs/heads/main/authentication/snipcart-authentication.yml
summary_line: http · 1 scheme
tags:
- E-Commerce
- Shopping Cart
- Orders
- Products
- Payments
- Webhooks
- Headless Commerce
- Jamstack
---
