---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Predoc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Predoc secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Predoc
provider_slug: predoc
scheme_count: 1
schemes:
- bearer_format: JWT
  description: 'JWT bearer authentication. Obtain a token by POSTing client_id and secret_key to /v1/auth/token; the response returns a JWT in the access_token field. Include it as `Authorization: Bearer <access_token>` on all subsequent requests. Tokens are valid for 5 minutes and must be refreshed prior to expiration.'
  name: bearerAuth
  scheme: bearer
  sources:
  - https://docs.predoc.ai/reference/authcontroller_signin_v1
  token_request:
    credentials:
    - client_id
    - secret_key
    endpoint: POST /v1/auth/token
    response_field: access_token
    ttl: 5 minutes
  type: http
slug: predoc-authentication
source_filename: predoc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.predoc.ai/reference/authcontroller_signin_v1\ndocs: https://docs.predoc.ai\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  bearer_format: JWT\n  token_endpoint: /v1/auth/token\n  token_ttl_seconds: 300\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  description: >-\n    JWT bearer authentication. Obtain a token by POSTing client_id and secret_key\n    to /v1/auth/token; the response returns a JWT in the access_token field. Include\n    it as `Authorization: Bearer <access_token>` on all subsequent requests. Tokens\n    are valid for 5 minutes and must be refreshed prior to expiration.\n  token_request:\n    endpoint: POST /v1/auth/token\n    credentials:\n    - client_id\n    - secret_key\n    response_field: access_token\n    ttl: 5 minutes\n  sources:\n  - https://docs.predoc.ai/reference/authcontroller_signin_v1\nnotes: >-\n  Predoc also supports SSO/SAML\
  \ integration with multi-factor authentication for\n  application (web app) access per the security & compliance documentation; the\n  Partner API itself uses short-lived JWT bearer tokens.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/predoc/refs/heads/main/authentication/predoc-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Healthcare
- Medical Records
- Health Information Exchange
- FHIR
- Clinical Data
- AI
- Interoperability
- EHR Integration
- Webhooks
- Clinical Research
---
