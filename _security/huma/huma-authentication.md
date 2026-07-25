---
api_key_in:
- header
api_specs:
- filename: huma-platform-openapi-original.yml
  format: yaml
  label: Huma Integration API
  slug: huma-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huma/refs/heads/main/openapi/huma-platform-openapi-original.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Huma Authentication
name_suffix: Authentication
oauth_flows: []
overview: Huma secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Huma
provider_slug: huma
scheme_count: 2
schemes:
- description: 'Hawk MAC authentication. Paste a full Authorization header value.


    Example:


    Authorization: Hawk id="userId:clientId", ts="<unix_ts>", nonce="<nonce>", mac="<mac>"[, hash="<hash>"][, ext="<ext>"]


    Note: Swagger UI cannot generate Hawk headers. Use your client to compute the MAC (e.g., with mohawk), then paste the full value here.'
  in: header
  name: Hawk Auth
  parameter: Authorization
  sources:
  - openapi/huma-platform-openapi-original.yml
  type: apiKey
- bearerFormat: JWT
  description: 'Use HTTP Bearer auth with a JWT.


    Send the token in the Authorization header:


    Authorization: Bearer <your_jwt_here>


    The token should contain standard claims plus projectId and clientId in user claims.'
  name: JWT Auth
  scheme: bearer
  sources:
  - openapi/huma-platform-openapi-original.yml
  type: http
slug: huma-authentication
source_filename: huma-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: derived\nsource: openapi/huma-platform-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: Hawk Auth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    Hawk MAC authentication. Paste a full Authorization header value.\n\n    Example:\n\n    Authorization: Hawk id=\"userId:clientId\", ts=\"<unix_ts>\", nonce=\"<nonce>\", mac=\"<mac>\"[, hash=\"<hash>\"][, ext=\"<ext>\"]\n\n    Note: Swagger UI cannot generate Hawk headers. Use your client to compute the MAC (e.g., with mohawk), then paste the full value here.\n  sources:\n  - openapi/huma-platform-openapi-original.yml\n- name: JWT Auth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    Use HTTP Bearer auth with a JWT.\n\n    Send the token in the Authorization header:\n\n    Authorization: Bearer <your_jwt_here>\n\n    The token should contain standard claims plus projectId and clientId\
  \ in user claims.\n  sources:\n  - openapi/huma-platform-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/huma/refs/heads/main/authentication/huma-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Healthcare
- United Kingdom
- Remote Patient Monitoring
- Telehealth
- Digital Health
- Clinical Trials
- SDK
- Medical Device Software
- Population Health
---
