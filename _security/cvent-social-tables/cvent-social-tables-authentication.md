---
api_key_in:
- header
api_specs:
- filename: cvent-social-tables-openapi.json
  format: json
  label: Social Tables Events API (Legacy)
  slug: events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-social-tables/refs/heads/main/openapi/cvent-social-tables-openapi.json
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Cvent Social Tables Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Cvent Social Tables secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Cvent Social Tables
provider_slug: cvent-social-tables
scheme_count: 3
schemes:
- description: OAuth
  flows:
  - authorizationUrl: https://auth.socialtables.com/oauth/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://auth.socialtables.com/oauth/token
  name: oauth2
  sources:
  - openapi/cvent-social-tables-openapi.json
  type: oauth2
- description: Social Tables User Token
  in: header
  name: user_token
  parameter: user_token
  sources:
  - openapi/cvent-social-tables-openapi.json
  type: apiKey
- description: Social Tables Partner Token
  in: header
  name: partner_token
  parameter: partner_token
  sources:
  - openapi/cvent-social-tables-openapi.json
  type: apiKey
slug: cvent-social-tables-authentication
source_filename: cvent-social-tables-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cvent-social-tables-openapi.json\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.socialtables.com/oauth/authorize\n    tokenUrl: https://auth.socialtables.com/oauth/token\n    scopes: 3\n  description: OAuth\n  sources:\n  - openapi/cvent-social-tables-openapi.json\n- name: user_token\n  type: apiKey\n  in: header\n  parameter: user_token\n  description: Social Tables User Token\n  sources:\n  - openapi/cvent-social-tables-openapi.json\n- name: partner_token\n  type: apiKey\n  in: header\n  parameter: partner_token\n  description: Social Tables Partner Token\n  sources:\n  - openapi/cvent-social-tables-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cvent-social-tables/refs/heads/main/authentication/cvent-social-tables-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- 3D Design
- Catering
- Diagramming
- Event Design
- Event Management
- Events
- Floor Plans
- Hospitality
- Hotel
- Meetings
- Seating
- Seating Charts
- Venues
---
