---
api_key_in: []
api_specs:
- filename: cariqa-openapi-original.yml
  format: yaml
  label: Cariqa Connect API
  slug: cariqa-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cariqa/refs/heads/main/openapi/cariqa-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Cariqa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cariqa secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cariqa
provider_slug: cariqa
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'JWT Authorization header using the Bearer scheme. Include `Authorization: Bearer [example key]` on every request to a protected endpoint.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/cariqa-openapi-original.yml
  type: http
slug: cariqa-authentication
source_filename: cariqa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/cariqa-openapi-original.yml\ndocs: https://docs.cariqa.com/authentication\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  token_format: JWT\n  onboarding: Tokens are issued by the Cariqa team through private channels during onboarding.\n  expiration: Access tokens are currently issued without an expiration date; they can be revoked on request, and multiple tokens can be issued for zero-downtime rotation.\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: \"JWT Authorization header using the Bearer scheme. Include `Authorization: Bearer [example key]` on every request to a protected endpoint.\"\n  sources:\n  - openapi/cariqa-openapi-original.yml\nnotes:\n- Credentials are environment-specific — development tokens do not work in production and vice versa.\n- 401 Unauthorized indicates the Authorization header is missing/malformed; 403 Forbidden indicates an\
  \ invalid or expired token.\nsecurity_recommendations:\n- Store secrets in a secure environment.\n- Use HTTPS for all API requests.\n- Rotate credentials periodically.\n- Do not log sensitive credentials.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cariqa/refs/heads/main/authentication/cariqa-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- EV Charging
- Electric Vehicles
- Payments
- Mobility
- e-Mobility
- Charge Point Operator
- Energy
---
