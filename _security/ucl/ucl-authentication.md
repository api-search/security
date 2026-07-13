---
api_key_in:
- query
api_specs:
- filename: uclapi.json
  format: json
  label: UCL API Room Bookings
  slug: roombookings
  spec_type: OpenAPI
  url: https://github.com/uclapi/uclapi-openapi/blob/master/uclapi.json
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Ucl Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: UCL secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: UCL
provider_slug: ucl
scheme_count: 2
schemes:
- description: This API requires you to pass your OAuth2 token as a query parameter called 'token'. Use the /authorize and /oauth/token endpoints to authorize a user and get this token.
  in: query
  name: OAuthToken
  parameter: token
  sources:
  - openapi/ucl-uclapi.yaml
  type: apiKey
- description: This API uses OAuth2 with the implicit grant flow. [More info](https://uclapi.com/docs#OAuthSecurity)
  flows:
  - authorizationUrl: /authorise
    flow: authorizationCode
    scopes: 2
    tokenUrl: /token
  name: OAuthSecurity
  sources:
  - openapi/ucl-uclapi.yaml
  type: oauth2
slug: ucl-authentication
source_filename: ucl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ucl-uclapi.yaml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuthToken\n  type: apiKey\n  in: query\n  parameter: token\n  description: This API requires you to pass your OAuth2 token as a query parameter called 'token'.\n    Use the /authorize and /oauth/token endpoints to authorize a user and get this token.\n  sources:\n  - openapi/ucl-uclapi.yaml\n- name: OAuthSecurity\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /authorise\n    tokenUrl: /token\n    scopes: 2\n  description: This API uses OAuth2 with the implicit grant flow. [More info](https://uclapi.com/docs#OAuthSecurity)\n  sources:\n  - openapi/ucl-uclapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ucl/refs/heads/main/authentication/ucl-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Education
- Higher Education
- University
- United Kingdom
- Open Data
- Research
- Library
- Timetable
---
