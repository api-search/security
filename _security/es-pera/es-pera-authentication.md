---
anonymous_access: false
api_key_in: []
api_specs:
- filename: es-pera-estado-api-openapi.yml
  format: yaml
  label: ES·pera API Estado API
  slug: es-pera-estado-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/es-pera/refs/heads/main/openapi/es-pera-estado-api-openapi.yml
- filename: es-pera-hospitales-api-openapi.yml
  format: yaml
  label: ES·pera API Hospitales API
  slug: es-pera-hospitales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/es-pera/refs/heads/main/openapi/es-pera-hospitales-api-openapi.yml
- filename: es-pera-listas-auton-micas-api-openapi.yml
  format: yaml
  label: ES·pera API Listas autonómicas API
  slug: es-pera-listas-auton-micas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/es-pera/refs/heads/main/openapi/es-pera-listas-auton-micas-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: derived
name: Es Pera Authentication
name_suffix: Authentication
oauth_flows: []
overview: ES·pera API declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: ES·pera API
provider_slug: es-pera
scheme_count: 0
schemes: []
slug: es-pera-authentication
source_filename: es-pera-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: derived\nsource: 'openapi/es-pera-openapi.json (security: []) + https://es-pera.org/metodologia/api/'\nname: ES·pera API authentication\nsummary: >-\n  The ES·pera public API is open and unauthenticated. The OpenAPI declares an\n  empty top-level security requirement (security: []) and no securitySchemes,\n  and the API documentation states operations require no authentication and are\n  read-only (GET/HEAD only). Access is instead governed by anonymous rate limits.\nschemes: []\nauth_required: false\npublic_access: true\nnotes:\n  - The whole surface is open read-only public open data; there is no API key,\n    OAuth, or token mechanism.\n  - Traffic is shaped by anonymous rate limits (120 req/min overall; 20 req/min\n    for /waiting/facets and /waiting/observations) rather than by credentials.\n    See rate-limits/es-pera-rate-limits.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/es-pera/refs/heads/main/authentication/es-pera-authentication.yml
summary_line: 0 schemes
tags:
- Healthcare
- Open Data
- Waiting Lists
- hospital activity
- Spain
- Public Sector
- Government Data
- SNS
---
