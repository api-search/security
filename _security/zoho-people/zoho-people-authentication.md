---
api_key_in: []
api_specs:
- filename: zoho-people-openapi.yml
  format: yaml
  label: Zoho People REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoho-people/refs/heads/main/openapi/zoho-people-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Zoho People Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Zoho People secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Zoho People
provider_slug: zoho-people
scheme_count: 1
schemes:
- description: 'Zoho Accounts OAuth 2.0 — Authorization Code grant. Access tokens

    live for 1 hour; refresh tokens are long-lived until revoked.

    Scope syntax is `ZOHOPEOPLE.<scope>.<operation>` where scope is

    one of employee, forms, dashboard, automation, timetracker,

    attendance, leave; operation is ALL, READ, CREATE, UPDATE, or

    DELETE.'
  flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: authorizationCode
    scopes: 13
    tokenUrl: https://accounts.zoho.com/oauth/v2/token
  name: ZohoOAuth2
  sources:
  - openapi/zoho-people-openapi.yml
  type: oauth2
slug: zoho-people-authentication
source_filename: zoho-people-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zoho-people-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: ZohoOAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n    tokenUrl: https://accounts.zoho.com/oauth/v2/token\n    scopes: 13\n  description: |-\n    Zoho Accounts OAuth 2.0 — Authorization Code grant. Access tokens\n    live for 1 hour; refresh tokens are long-lived until revoked.\n    Scope syntax is `ZOHOPEOPLE.<scope>.<operation>` where scope is\n    one of employee, forms, dashboard, automation, timetracker,\n    attendance, leave; operation is ALL, READ, CREATE, UPDATE, or\n    DELETE.\n  sources:\n  - openapi/zoho-people-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoho-people/refs/heads/main/authentication/zoho-people-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- HR
- HRMS
- Human Resources
- HRIS
- Employee Management
- Attendance
- Leave Management
- Time Tracking
- Performance Management
- Onboarding
- Zoho
- OAuth 2.0
---
