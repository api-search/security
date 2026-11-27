---
anonymous_access: false
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: G86 Racing Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: G86 Racing secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: G86 Racing
provider_slug: g86racing-com
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://api.g86racing.com/oauth/authorize
    flow: authorizationCode
    scopes: 6
    tokenUrl: https://api.g86racing.com/oauth/token
  name: oauth
  sources:
  - openapi/g86racing-com-openapi.json
  type: oauth2
slug: g86racing-com-authentication
source_filename: g86racing-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: derived\nsource: openapi/g86racing-com-openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.g86racing.com/oauth/authorize\n    tokenUrl: https://api.g86racing.com/oauth/token\n    scopes: 6\n  sources:\n  - openapi/g86racing-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/g86racing-com/authentication/g86racing-com-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Motorsports
- Telemetry
- Lap Timing
- Mobile App
- Data Export
---
