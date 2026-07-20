---
api_key_in: []
api_specs:
- filename: instock-openapi.json
  format: json
  label: Instock API
  slug: instock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instock/refs/heads/main/openapi/instock-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Instock Authentication
name_suffix: Authentication
oauth_flows: []
overview: Instock secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Instock
provider_slug: instock
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/instock-openapi.json
  type: http
slug: instock-authentication
source_filename: instock-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/instock-openapi.json\ndocs: https://instock.com/en/docs/api/\ndetail: >-\n  Instock API authenticates with a Bearer token (JWT). The token must be present\n  in the Authorization header of every request; requests without authentication\n  fail, and HTTPS is required. The token grants full access to all resources and\n  methods of the Instock API for its client. Tokens are currently issued by\n  Instock and supplied to API users during onboarding (no self-service token\n  provisioning / OAuth flow is documented). There are no scopes documented — the\n  token is all-or-nothing per client.\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  token_header: Authorization\n  token_format: JWT\n  self_service: false\n  issued_by: Instock (during onboarding)\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/instock-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instock/refs/heads/main/authentication/instock-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Robotics
- Warehouse Automation
- Fulfillment
- Logistics
- ASRS
- Supply Chain
- Inventory Management
---
