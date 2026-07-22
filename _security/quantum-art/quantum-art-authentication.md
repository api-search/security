---
api_key_in: []
api_specs:
- filename: quantum-art-qaas-openapi-original.json
  format: json
  label: QaaS Backend API
  slug: qaas-backend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quantum-art/refs/heads/main/openapi/quantum-art-qaas-openapi-original.json
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Quantum Art Authentication
name_suffix: Authentication
oauth_flows: []
overview: Quantum Art secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Quantum Art
provider_slug: quantum-art
scheme_count: 2
schemes:
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/quantum-art-qaas-openapi-original.json
  type: http
- in: header
  name: APIKey
  sources:
  - https://qaas.quantum-art.tech/documentation
  type: apiKey
  x-managed-by:
  - GET /api/profile/api-key
  - POST /api/profile/api-key/regenerate
  x-note: Account API key issued/rotated from the user profile; presented as a bearer credential to the API. Not declared as a distinct OpenAPI securityScheme.
slug: quantum-art-authentication
source_filename: quantum-art-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/quantum-art-qaas-openapi-original.json\ndocs: https://qaas.quantum-art.tech/documentation\nsummary:\n  types:\n  - http\n  - apiKey\n  http_schemes:\n  - bearer\n  notes: >-\n    The QaaS Backend API authenticates requests with a bearer token\n    (Authorization: Bearer <token>). Interactive sessions obtain a JWT via\n    /auth/login (with optional MFA verification at /auth/login/verify-mfa).\n    Programmatic access uses a per-account API key managed from the profile\n    surface (GET /api/profile/api-key, POST /api/profile/api-key/regenerate).\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/quantum-art-qaas-openapi-original.json\n- name: APIKey\n  type: apiKey\n  in: header\n  x-managed-by:\n  - GET /api/profile/api-key\n  - POST /api/profile/api-key/regenerate\n  x-note: >-\n    Account API key issued/rotated from the user profile; presented as a bearer\n    credential to the\
  \ API. Not declared as a distinct OpenAPI securityScheme.\n  sources:\n  - https://qaas.quantum-art.tech/documentation\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quantum-art/refs/heads/main/authentication/quantum-art-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- Company
- Quantum Computing
- Quantum as a Service
- Qiskit
- Developer Tools
- Machine Learning
- Optimization
- Finance
- Chemistry
---
