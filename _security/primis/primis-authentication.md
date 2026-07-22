---
api_key_in: []
api_specs:
- filename: primis-openapi-original.json
  format: json
  label: Primis REST API
  slug: primis-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/primis/refs/heads/main/openapi/primis-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Primis Authentication
name_suffix: Authentication
oauth_flows: []
overview: PRIMIS secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PRIMIS
provider_slug: primis
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/primis-openapi-original.json
  type: http
slug: primis-authentication
source_filename: primis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/primis-openapi-original.json\ndocs: https://api.primis.cx/api-docs\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  bearer_format: JWT\nnotes: >-\n  The Primis REST API is served over HTTPS and requires an Authentication Token\n  on all requests. The OpenAPI declares a single HTTP bearer scheme\n  (bearerAuth, bearerFormat JWT); the published API docs describe three token\n  types carried in the Authorization header. The spec's securityScheme declares\n  type \"https\" (a typo for the OpenAPI \"http\" type) — captured here as the\n  intended http/bearer profile.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/primis-openapi-original.json\ntoken_types:\n- name: JWT\n  description: Provided on successful login of an account (POST /auth/login). Must be set in the Authorization header prepended with \"Bearer \".\n  header: 'Authorization: Bearer <jwt>'\n\
  - name: Retailer API Key\n  description: Provided when adding an API Key to an integration. Sent in the Authorization header WITHOUT the \"Bearer \" prefix.\n  header: 'Authorization: <retailer-api-key>'\n- name: CMS API Key\n  description: Provided by a Primis Developer upon request; used for communication between Primis services and external services not associated with a specific retailer. Sent WITHOUT the \"Bearer \" prefix.\n  header: 'Authorization: <cms-api-key>'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/primis/refs/heads/main/authentication/primis-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- eCommerce
- Logistics
- Shipping
- Returns
- Order Tracking
- Post-Purchase
- Customer Experience
- Fulfillment
---
