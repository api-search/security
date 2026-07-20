---
api_key_in: []
api_specs:
- filename: authlete-openapi-original.yml
  format: yaml
  label: Authlete API
  slug: authlete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authlete/refs/heads/main/openapi/authlete-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Authlete Authentication
name_suffix: Authentication
oauth_flows: []
overview: Authlete secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Authlete
provider_slug: authlete
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Authenticate every request with a **Service Access Token** or **Organization Token**.

    Set the token value in the `Authorization: Bearer <token>` header.


    **Service Access Token**: Scoped to a single service. Use when automating service-level configuration or runtime flows.


    **Organization Token**: Scoped to the organization; inherits permissions across services. Use for org-wide automation or when'
  name: bearer
  scheme: bearer
  sources:
  - openapi/authlete-openapi-original.yml
  type: http
slug: authlete-authentication
source_filename: authlete-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/authlete-openapi-original.yml\ndocs: https://docs.authlete.com/\npermissions_model: >-\n  Access tokens are minted in the Authlete console (or provisioning APIs) with permission\n  strings that gate which operations they may call, e.g. service.read, service.write,\n  client.read, client.write. Service Access Tokens are limited to one service; Organization\n  Tokens inherit permissions across all services in the organization.\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    Authenticate every request with a **Service Access Token** or **Organization Token**.\n    Set the token value in the `Authorization: Bearer <token>` header.\n\n    **Service Access Token**: Scoped to a single service. Use when automating service-level configuration or runtime flows.\n\n    **Organization Token**: Scoped to the organization; inherits permissions across\
  \ services. Use for org-wide automation or when\n  sources:\n  - openapi/authlete-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/authlete/refs/heads/main/authentication/authlete-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- OAuth 2.0
- OpenID Connect
- Authentication
- Authorization
- Identity
- API Security
- FAPI
- Verifiable Credentials
- CIBA
---
