---
api_key_in: []
api_specs:
- filename: keyo-openapi.yml
  format: yaml
  label: Keyo REST API
  slug: keyo-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keyo/refs/heads/main/openapi/keyo-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Keyo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Keyo secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Keyo
provider_slug: keyo
scheme_count: 2
schemes:
- name: Basic
  scheme: Basic
  sources:
  - openapi/keyo-openapi.yml
  type: http
  usage: Token endpoint only (POST /oauth/token/) - base64 client_id:client_secret
- bearerFormat: <access-token>
  name: Bearer
  scheme: bearer
  sources:
  - openapi/keyo-openapi.yml
  type: http
  usage: All protected resource requests
slug: keyo-authentication
source_filename: keyo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/keyo-openapi.yml\ndocs: https://developers.keyo.co/rest-api/authentication\nsummary:\n  types:\n  - http\n  model: oauth2-client-credentials\n  notes: >-\n    Keyo implements the OAuth 2.0 Client Credentials flow for server-to-server\n    integrations. A base64-encoded secret key (client_id:client_secret) is\n    created on the organization dashboard API credentials page and presented as\n    `Authorization: Basic <secret-key>` to POST /oauth/token/ to obtain a\n    short-lived bearer access token. All subsequent API calls send\n    `Authorization: Bearer <access-token>`. Applications must handle token\n    expiration/renewal.\nschemes:\n- name: Basic\n  type: http\n  scheme: Basic\n  usage: Token endpoint only (POST /oauth/token/) - base64 client_id:client_secret\n  sources:\n  - openapi/keyo-openapi.yml\n- name: Bearer\n  type: http\n  scheme: bearer\n  bearerFormat: <access-token>\n  usage: All protected resource\
  \ requests\n  sources:\n  - openapi/keyo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keyo/refs/heads/main/authentication/keyo-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Biometrics
- Identity
- Authentication
- Palm Recognition
- Access Control
- Payments
- Identity Verification
---
