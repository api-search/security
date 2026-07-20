---
api_key_in: []
api_specs:
- filename: catchpoint-systems-rest-api-v2-openapi.json
  format: json
  label: Catchpoint REST API v2
  slug: catchpoint-rest-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/catchpoint-systems/refs/heads/main/openapi/catchpoint-systems-rest-api-v2-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Catchpoint Systems Authentication
name_suffix: Authentication
oauth_flows: []
overview: Catchpoint Systems secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Catchpoint Systems
provider_slug: catchpoint-systems
scheme_count: 1
schemes:
- bearerFormat: JWT
  header: Authorization
  in: header
  name: bearer
  scheme: bearer
  sources:
  - openapi/catchpoint-systems-rest-api-v2-openapi.json
  type: http
slug: catchpoint-systems-authentication
source_filename: catchpoint-systems-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/catchpoint-systems-rest-api-v2-openapi.json\ndocs: https://docs.catchpoint.com/docs/rest-api-v2-guide\nsummary:\n  types:\n  - http\n  scheme: bearer\n  bearer_format: JWT\nnotes: >-\n  Catchpoint REST API v2 authenticates with a bearer (JWT) token passed in the Authorization header\n  (Authorization: Bearer <token>). API credentials (a REST API key/client id and secret) are generated\n  from the Catchpoint Portal under API settings; the credentials are exchanged for a short-lived bearer\n  token that is then sent on every request. There are no OAuth2 scopes declared in the spec.\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  in: header\n  header: Authorization\n  sources:\n  - openapi/catchpoint-systems-rest-api-v2-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/catchpoint-systems/refs/heads/main/authentication/catchpoint-systems-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Monitoring
- Observability
- Internet Performance Monitoring
- Synthetic Monitoring
- Real User Monitoring
- Network Monitoring
- Digital Experience Monitoring
- APIs
---
