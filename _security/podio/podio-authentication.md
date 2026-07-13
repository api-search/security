---
api_key_in: []
api_specs:
- filename: podio-openapi.yml
  format: yaml
  label: Podio REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podio/refs/heads/main/openapi/podio-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Podio Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Podio secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Podio
provider_slug: podio
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://podio.com/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://api.podio.com/oauth/token/v2
  name: oauth2Authorization
  sources:
  - openapi/podio-openapi.yml
  type: oauth2
- description: 'Podio also accepts bearer-style tokens via `Authorization: OAuth2 <access_token>`.'
  name: oauth2Token
  scheme: bearer
  sources:
  - openapi/podio-openapi.yml
  type: http
slug: podio-authentication
source_filename: podio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/podio-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2Authorization\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://podio.com/oauth/authorize\n    tokenUrl: https://api.podio.com/oauth/token/v2\n    scopes: 0\n  sources:\n  - openapi/podio-openapi.yml\n- name: oauth2Token\n  type: http\n  scheme: bearer\n  description: 'Podio also accepts bearer-style tokens via `Authorization: OAuth2 <access_token>`.'\n  sources:\n  - openapi/podio-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/podio/refs/heads/main/authentication/podio-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Work Management
- Collaboration
- Project Management
- CRM
- Workflow
- Custom Apps
---
