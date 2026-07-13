---
api_key_in: []
api_specs:
- filename: whimsical-openapi.yml
  format: yaml
  label: Whimsical API (Beta)
  slug: whimsical-api-beta
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whimsical/refs/heads/main/openapi/whimsical-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Whimsical Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Whimsical secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Whimsical
provider_slug: whimsical
scheme_count: 1
schemes:
- description: OAuth 2.1 authorization (contact Whimsical support for client credentials)
  flows:
  - authorizationUrl: https://whimsical.com/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://whimsical.com/oauth/token
  name: OAuth2
  sources:
  - openapi/whimsical-openapi.yml
  type: oauth2
slug: whimsical-authentication
source_filename: whimsical-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/whimsical-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://whimsical.com/oauth/authorize\n    tokenUrl: https://whimsical.com/oauth/token\n    scopes: 0\n  description: OAuth 2.1 authorization (contact Whimsical support for client credentials)\n  sources:\n  - openapi/whimsical-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whimsical/refs/heads/main/authentication/whimsical-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Collaboration
- Diagramming
- Flowcharts
- Wireframes
- Mind Maps
---
