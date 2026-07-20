---
api_key_in: []
api_specs:
- filename: humanapi-admin-openapi.yml
  format: yaml
  label: Human API - Admin API
  slug: human-api-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanapi/refs/heads/main/openapi/humanapi-admin-openapi.yml
- filename: humanapi-auth-openapi.yml
  format: yaml
  label: Human API - HAPI Auth Public
  slug: human-api-hapi-auth-public
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanapi/refs/heads/main/openapi/humanapi-auth-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Humanapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: HumanAPI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: HumanAPI
provider_slug: humanapi
scheme_count: 1
schemes:
- applies_to: openapi/humanapi-admin-openapi.yml
  bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/humanapi-admin-openapi.yml
  type: http
slug: humanapi-authentication
source_filename: humanapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/humanapi-admin-openapi.yml, openapi/humanapi-auth-openapi.yml, https://reference.humanapi.co/docs/admin-api\ndocs: https://reference.humanapi.co\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  model: >-\n    Bearer JWT. A client exchanges its client_id/client_secret at the HAPI Auth\n    Public token endpoints (auth.humanapi.co) for a JWT, then calls the Admin API\n    (admin.humanapi.co) with Authorization: Bearer <jwt>.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  applies_to: openapi/humanapi-admin-openapi.yml\n  sources:\n  - openapi/humanapi-admin-openapi.yml\ntoken_endpoints:\n- url: https://auth.humanapi.co/v1/admin/token\n  client_type: admin\n  request_fields: [client_id, client_secret, type]\n  description: Admin API client-type token\n- url: https://auth.humanapi.co/v1/connect/token\n  client_type: connect\n  request_fields: [client_id, client_user_id,\
  \ client_secret, client_user_email, type, extra_scopes]\n  description: Public Connect token; supports per-user tokens and extra_scopes\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/humanapi/refs/heads/main/authentication/humanapi-authentication.yml
summary_line: http · 1 scheme
tags:
- Health
- Healthcare
- Health Data
- Medical Records
- Insurance
- Underwriting
- Wellness
- Data Aggregation
- Reports
- FHIR-adjacent
---
