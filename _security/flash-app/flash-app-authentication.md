---
api_key_in: []
api_specs:
- filename: flash-app-expense-openapi-original.json
  format: json
  label: Flash Expense API
  slug: flash-expense-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flash-app/refs/heads/main/openapi/flash-app-expense-openapi-original.json
auth_types:
- credential-login
description: ''
kind: authentication
layout: security
method: searched
name: Flash App Authentication
name_suffix: Authentication
oauth_flows: []
overview: Flash App secures its APIs with credential-login across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Flash App
provider_slug: flash-app
scheme_count: 1
schemes:
- location: request body
  name: integration-user-login
  operation: login
  parameters:
  - description: Numeric company identifier the integration user belongs to
    name: id_empresa
  - description: Email of the integration user (usuario integrador)
    name: email
  - description: Password of the integration user
    name: senha
  - description: reCAPTCHA token accompanying the login request
    name: recaptcha
  sources:
  - openapi/flash-app-expense-openapi-original.json
  type: credential-login
slug: flash-app-authentication
source_filename: flash-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/flash-app-expense-openapi-original.json\ndocs: https://flashapp.readme.io/reference/login\nsummary:\n  types:\n  - credential-login\n  api_key_in: []\n  oauth2_flows: []\n  declared_security_schemes: 0\nnotes: >-\n  The published OpenAPI 3.1 definition for the Flash Expense API declares an\n  empty components.securitySchemes object and an empty global security\n  requirement, so there is no machine-readable auth scheme to derive. The\n  documented model is instead a credential login: POST /login is called with\n  id_empresa, email and senha for a dedicated \"usuario integrador\" (integration\n  user) plus a recaptcha field, and the resulting session credential is used for\n  subsequent integration calls such as POST /integration/user. Flash does not\n  publish an OAuth 2.0 or OpenID Connect surface, an API key scheme, or a scopes\n  reference, so scopes/ is intentionally absent for this provider.\nschemes:\n- name:\
  \ integration-user-login\n  type: credential-login\n  operation: login\n  location: request body\n  parameters:\n  - name: id_empresa\n    description: Numeric company identifier the integration user belongs to\n  - name: email\n    description: Email of the integration user (usuario integrador)\n  - name: senha\n    description: Password of the integration user\n  - name: recaptcha\n    description: reCAPTCHA token accompanying the login request\n  sources:\n  - openapi/flash-app-expense-openapi-original.json\ngaps:\n- No securitySchemes declared in the OpenAPI definition.\n- Token format, lifetime, refresh and transport header for the credential\n  returned by POST /login are not documented publicly.\n- No OAuth 2.0 / OIDC surface and no scopes or permissions reference published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flash-app/refs/heads/main/authentication/flash-app-authentication.yml
summary_line: credential-login · 1 scheme
tags:
- Company
- Human Resources
- Employee Benefits
- Expense Management
- Payments
- Corporate Cards
- Payroll
- Fintech
- Brazil
- HR Tech
---
