---
api_key_in: []
api_specs:
- filename: kinde-management-api-openapi.yml
  format: yaml
  label: Kinde Management API
  slug: kinde-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde/refs/heads/main/openapi/kinde-management-api-openapi.yml
- filename: kinde-frontend-api-openapi.yml
  format: yaml
  label: Kinde Account API
  slug: kinde-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde/refs/heads/main/openapi/kinde-frontend-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Kinde Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kinde secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kinde
provider_slug: kinde
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: To access these endpoints, you will need to use a user token. This can be obtained when your users sign in via the methods you've setup in Kinde (e.g. Google, passwordless, etc). Find this using the getToken command in the relevant SDK.
  name: kindeBearerAuth
  scheme: bearer
  sources:
  - openapi/kinde-frontend-api-openapi.yml
  - openapi/kinde-management-api-openapi.yml
  type: http
slug: kinde-authentication
source_filename: kinde-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kinde-frontend-api-openapi.yml, openapi/kinde-management-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: kindeBearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: To access these endpoints, you will need to use a user token. This can be obtained\n    when your users sign in via the methods you've setup in Kinde (e.g. Google, passwordless,\n    etc). Find this using the getToken command in the relevant SDK.\n  sources:\n  - openapi/kinde-frontend-api-openapi.yml\n  - openapi/kinde-management-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kinde/refs/heads/main/authentication/kinde-authentication.yml
summary_line: http · 1 scheme
tags:
- Authentication
- Authorization
- Customer Identity
- Identity Management
- OAuth
- OpenID Connect
- Single Sign-On
- Multi-Factor Authentication
- Role-Based Access Control
- Feature Flags
- Billing
- B2B
- SaaS
- Developer Platform
---
