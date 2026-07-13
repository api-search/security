---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Ford Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Ford secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Ford
provider_slug: ford
scheme_count: 2
schemes:
- description: OAuth 2.0 authorization-code grant brokered through Ford's identity service
  flows:
  - authorizationUrl: https://fordconnect.cv.ford.com/common/login
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://dah2vb2cprod.b2clogin.com/914d88b1-3523-4bf6-9be4-1b96b4f6f919/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/ford-openapi.yml
  type: oauth2
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ford-openapi.yml
  type: http
slug: ford-authentication
source_filename: ford-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ford-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://fordconnect.cv.ford.com/common/login\n    tokenUrl: https://dah2vb2cprod.b2clogin.com/914d88b1-3523-4bf6-9be4-1b96b4f6f919/oauth2/v2.0/token\n    scopes: 1\n  description: OAuth 2.0 authorization-code grant brokered through Ford's identity service\n  sources:\n  - openapi/ford-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/ford-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ford/refs/heads/main/authentication/ford-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Automobiles
- Cars
- Vehicles
---
