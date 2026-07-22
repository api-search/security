---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Spaceiq Authentication
name_suffix: Authentication
oauth_flows: []
overview: SpaceIQ secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SpaceIQ
provider_slug: spaceiq
scheme_count: 1
schemes:
- description: Admin/IT-generated access token. Required on every request to the GraphQL endpoint https://api.spaceiq.com/queries. Requests without a valid token return HTTP 401 with body {"error":"access_token does not correspond to user"}.
  format: 'Authorization: bearer: <token>  (JWT; header value as documented)'
  in: header
  name: accessToken
  parameter: Authorization
  sources:
  - https://developer.spaceiq.com/
  type: apiKey
slug: spaceiq-authentication
source_filename: spaceiq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.spaceiq.com/\ndocs: https://developer.spaceiq.com/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  notes: >-\n    SpaceIQ (SiQ) uses a single long-lived access token passed as a bearer token\n    in the HTTP Authorization header. The token is a JWT generated inside the SiQ\n    web application by a user with access level \"Admin\" or \"IT\" from the\n    Integration page (General Integrations > API > Activate). Multiple tokens can\n    be issued for different applications and individually disabled. A lost token\n    cannot be recovered; the integration instance must be disabled and re-created.\n    There is no OAuth authorization/token endpoint and no scope surface.\nschemes:\n- name: accessToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: >-\n    Authorization: bearer: <token>  (JWT; header value as documented)\n  description: >-\n    Admin/IT-generated\
  \ access token. Required on every request to the GraphQL\n    endpoint https://api.spaceiq.com/queries. Requests without a valid token\n    return HTTP 401 with body {\"error\":\"access_token does not correspond to user\"}.\n  sources:\n  - https://developer.spaceiq.com/\ntoken_management:\n  generated_in: SiQ web application > Integration page > General Integrations > API\n  required_role:\n  - Admin\n  - IT\n  revocable: true\n  recoverable: false\n  multiple_tokens: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spaceiq/refs/heads/main/authentication/spaceiq-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Workplace Management
- Space Management
- Facilities Management
- Desk Booking
- Hoteling
- Meeting Rooms
- Occupancy Analytics
- Real Estate
- Floorplans
- GraphQL
- IWMS
- Eptura
---
