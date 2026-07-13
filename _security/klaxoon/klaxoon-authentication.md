---
api_key_in: []
api_specs:
- filename: klaxoon-openapi.yml
  format: yaml
  label: Klaxoon API
  slug: klaxoon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klaxoon/refs/heads/main/openapi/klaxoon-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Klaxoon Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Klaxoon secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Klaxoon
provider_slug: klaxoon
scheme_count: 1
schemes:
- description: OAuth 2.0 authorization-code flow against Klaxoon. Scopes are issued per integration via the Klaxoon developer portal.
  flows:
  - authorizationUrl: https://access.klaxoon.com/auth
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://access.klaxoon.com/token
  name: OAuth2
  sources:
  - openapi/klaxoon-openapi.yml
  type: oauth2
slug: klaxoon-authentication
source_filename: klaxoon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/klaxoon-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://access.klaxoon.com/auth\n    tokenUrl: https://access.klaxoon.com/token\n    scopes: 0\n  description: OAuth 2.0 authorization-code flow against Klaxoon. Scopes are issued per integration\n    via the Klaxoon developer portal.\n  sources:\n  - openapi/klaxoon-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klaxoon/refs/heads/main/authentication/klaxoon-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Collaboration
- Meetings
- Productivity
- Team Collaboration
- Workshops
- Brainstorming
- Whiteboard
---
