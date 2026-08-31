---
api_key_in: []
api_specs:
- filename: easyship-addresses-api-openapi.yml
  format: yaml
  label: Easyship Addresses API
  slug: easyship-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/easyship/refs/heads/main/openapi/easyship-addresses-api-openapi.yml
- filename: easyship-labels-api-openapi.yml
  format: yaml
  label: Easyship Labels API
  slug: easyship-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/easyship/refs/heads/main/openapi/easyship-labels-api-openapi.yml
- filename: easyship-pickups-api-openapi.yml
  format: yaml
  label: Easyship Pickups API
  slug: easyship-pickups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/easyship/refs/heads/main/openapi/easyship-pickups-api-openapi.yml
- filename: easyship-rates-api-openapi.yml
  format: yaml
  label: Easyship Rates API
  slug: easyship-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/easyship/refs/heads/main/openapi/easyship-rates-api-openapi.yml
- filename: easyship-shipments-api-openapi.yml
  format: yaml
  label: Easyship Shipments API
  slug: easyship-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/easyship/refs/heads/main/openapi/easyship-shipments-api-openapi.yml
- filename: easyship-trackings-api-openapi.yml
  format: yaml
  label: Easyship Trackings API
  slug: easyship-trackings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/easyship/refs/heads/main/openapi/easyship-trackings-api-openapi.yml
- filename: easyship-webhooks-api-openapi.yml
  format: yaml
  label: Easyship Webhooks API
  slug: easyship-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/easyship/refs/heads/main/openapi/easyship-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Easyship Authentication
name_suffix: Authentication
oauth_flows: []
overview: Easyship secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Easyship
provider_slug: easyship
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/easyship-openapi.yml
  type: http
slug: easyship-authentication
source_filename: easyship-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/easyship-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/easyship-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/easyship/refs/heads/main/authentication/easyship-authentication.yml
summary_line: http · 1 scheme
tags:
- Shipping
- Logistics
- E-Commerce
- Fulfillment
- CrossBorder
---
