---
api_key_in: []
api_specs:
- filename: axle-energy-openapi-original.json
  format: json
  label: Axle API
  slug: axle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axle-energy/refs/heads/main/openapi/axle-energy-openapi-original.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Axle Energy Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Axle Energy secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Axle Energy
provider_slug: axle-energy
scheme_count: 1
schemes:
- flows:
  - flow: password
    scopes: 0
    tokenUrl: auth/token-form
  name: OAuth2PasswordBearer
  sources:
  - openapi/axle-energy-openapi-original.json
  type: oauth2
slug: axle-energy-authentication
source_filename: axle-energy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/axle-energy-openapi-original.json\ndocs: https://docs.axle.energy/api-reference/auth/token-form\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - password\n  detail: >-\n    Token-based auth. Exchange API credentials (username/password) for a bearer token via\n    POST /auth/token-form. Organisation tokens are valid 1 hour. Component tokens\n    (POST /auth/component-token) are site-scoped and valid 24 hours for end-user sessions.\n    Send the token as `Authorization: Bearer <token>`.\nschemes:\n- name: OAuth2PasswordBearer\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: auth/token-form\n    scopes: 0\n  sources:\n  - openapi/axle-energy-openapi-original.json\ntoken_types:\n  - name: organisation-token\n    endpoint: POST /auth/token-form\n    ttl: 1h\n    docs: https://docs.axle.energy/api-reference/auth/token-form\n  - name: component-token\n    endpoint: POST /auth/component-token\n    ttl: 24h\n\
  \    scope: site\n    docs: https://docs.axle.energy/api-reference/auth/component-token\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axle-energy/refs/heads/main/authentication/axle-energy-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Energy
- Flexibility
- Virtual Power Plant
- Electric Vehicles
- Smart Charging
- Batteries
- Demand Response
- Grid
- Sustainability
---
