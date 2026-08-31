---
api_key_in:
- header
api_specs:
- filename: petpooja-menu-api-openapi.yml
  format: yaml
  label: Petpooja Menu API
  slug: petpooja-menu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petpooja/refs/heads/main/openapi/petpooja-menu-api-openapi.yml
- filename: petpooja-orders-api-openapi.yml
  format: yaml
  label: Petpooja Orders API
  slug: petpooja-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petpooja/refs/heads/main/openapi/petpooja-orders-api-openapi.yml
- filename: petpooja-stock-api-openapi.yml
  format: yaml
  label: Petpooja Stock API
  slug: petpooja-stock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petpooja/refs/heads/main/openapi/petpooja-stock-api-openapi.yml
- filename: petpooja-stores-api-openapi.yml
  format: yaml
  label: Petpooja Stores API
  slug: petpooja-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petpooja/refs/heads/main/openapi/petpooja-stores-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Petpooja Authentication
name_suffix: Authentication
oauth_flows: []
overview: Petpooja secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Petpooja
provider_slug: petpooja
scheme_count: 1
schemes:
- description: Petpooja issues an app-key, app-secret, and access-token per integration and a restID per mapped restaurant. Menu/restaurant calls send app-key, app-secret, and access-token as request headers; the save_order call sends app_key, app_secret, and access_token in the request body. Credentials are obtained by emailing support@petpooja.com.
  in: header
  name: PetpoojaAuthHeaders
  parameter: access-token
  sources:
  - openapi/petpooja-openapi.yml
  type: apiKey
slug: petpooja-authentication
source_filename: petpooja-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/petpooja-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: PetpoojaAuthHeaders\n  type: apiKey\n  in: header\n  parameter: access-token\n  description: Petpooja issues an app-key, app-secret, and access-token per integration and\n    a restID per mapped restaurant. Menu/restaurant calls send app-key, app-secret, and access-token\n    as request headers; the save_order call sends app_key, app_secret, and access_token in the\n    request body. Credentials are obtained by emailing support@petpooja.com.\n  sources:\n  - openapi/petpooja-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/petpooja/refs/heads/main/authentication/petpooja-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Restaurant
- POS
- Online Ordering
- Menus
- Food Delivery
---
