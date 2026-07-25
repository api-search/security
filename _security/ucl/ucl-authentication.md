---
api_key_in:
- query
api_specs:
- filename: ucl-analytics-api-openapi.yml
  format: yaml
  label: UCL Analytics API
  slug: ucl-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucl/refs/heads/main/openapi/ucl-analytics-api-openapi.yml
- filename: ucl-oauth-api-openapi.yml
  format: yaml
  label: UCL OAuth API
  slug: ucl-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucl/refs/heads/main/openapi/ucl-oauth-api-openapi.yml
- filename: ucl-resources-api-openapi.yml
  format: yaml
  label: UCL Resources API
  slug: ucl-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucl/refs/heads/main/openapi/ucl-resources-api-openapi.yml
- filename: ucl-room-bookings-api-openapi.yml
  format: yaml
  label: UCL Room Bookings API
  slug: ucl-room-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucl/refs/heads/main/openapi/ucl-room-bookings-api-openapi.yml
- filename: ucl-search-api-openapi.yml
  format: yaml
  label: UCL Search API
  slug: ucl-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucl/refs/heads/main/openapi/ucl-search-api-openapi.yml
- filename: ucl-timetable-api-openapi.yml
  format: yaml
  label: UCL Timetable API
  slug: ucl-timetable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucl/refs/heads/main/openapi/ucl-timetable-api-openapi.yml
- filename: ucl-workspaces-api-openapi.yml
  format: yaml
  label: UCL Workspaces API
  slug: ucl-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucl/refs/heads/main/openapi/ucl-workspaces-api-openapi.yml
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
