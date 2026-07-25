---
api_key_in: []
api_specs:
- filename: button-accounts-api-openapi.yml
  format: yaml
  label: Button Accounts API
  slug: button-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/button/refs/heads/main/openapi/button-accounts-api-openapi.yml
- filename: button-brands-api-api-openapi.yml
  format: yaml
  label: Button Brands Api API
  slug: button-brands-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/button/refs/heads/main/openapi/button-brands-api-api-openapi.yml
- filename: button-create-api-openapi.yml
  format: yaml
  label: Button Create API
  slug: button-create-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/button/refs/heads/main/openapi/button-create-api-openapi.yml
- filename: button-links-api-api-openapi.yml
  format: yaml
  label: Button Links Api API
  slug: button-links-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/button/refs/heads/main/openapi/button-links-api-api-openapi.yml
- filename: button-offers-api-openapi.yml
  format: yaml
  label: Button Offers API
  slug: button-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/button/refs/heads/main/openapi/button-offers-api-openapi.yml
- filename: button-transactions-api-openapi.yml
  format: yaml
  label: Button Transactions API
  slug: button-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/button/refs/heads/main/openapi/button-transactions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Button Authentication
name_suffix: Authentication
oauth_flows: []
overview: Button secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Button
provider_slug: button
scheme_count: 1
schemes:
- name: sec0
  scheme: basic
  sources:
  - openapi/button-billing-api-openapi.json
  - openapi/button-brands-api-openapi.json
  - openapi/button-links-api-openapi.json
  - openapi/button-offers-api-openapi.json
  - openapi/button-shortlink-api-openapi.json
  type: http
slug: button-authentication
source_filename: button-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/button-billing-api-openapi.json, openapi/button-brands-api-openapi.json, openapi/button-links-api-openapi.json,\n  openapi/button-offers-api-openapi.json, openapi/button-shortlink-api-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: sec0\n  type: http\n  scheme: basic\n  sources:\n  - openapi/button-billing-api-openapi.json\n  - openapi/button-brands-api-openapi.json\n  - openapi/button-links-api-openapi.json\n  - openapi/button-offers-api-openapi.json\n  - openapi/button-shortlink-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/button/refs/heads/main/authentication/button-authentication.yml
summary_line: http · 1 scheme
tags:
- Commerce
- Affiliate Marketing
- Mobile
- Attribution
- Deep Linking
- Retail Media
- Analytics
- Advertising
- Links
---
