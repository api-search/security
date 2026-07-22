---
api_key_in:
- header
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Plangrid Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: PlanGrid secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: PlanGrid
provider_slug: plangrid
scheme_count: 2
schemes:
- description: 'OAuth 2.0 for authenticating and authorizing PlanGrid users on behalf of an application. Applications must be registered with PlanGrid (contact developers@plangrid.com) with an application name, logo, and list of redirect URIs. Access tokens are sent as "Authorization: Bearer <access_token>".'
  flows:
  - authorizationUrl: https://io.plangrid.com/oauth/authorize
    flow: authorizationCode
    refresh: true
    tokenUrl: https://io.plangrid.com/oauth/token
  - authorizationUrl: https://io.plangrid.com/oauth/authorize
    flow: implicit
  name: OAuth2
  scopes:
  - write:projects
  - read:profile
  type: oauth2
- description: HTTP Basic authentication where the API key is sent as the username and the password is left blank (e.g. curl -u API_KEY:). 401 is returned when the API key is missing, 403 when the key is invalid or deactivated.
  in: header
  name: ApiKeyBasic
  scheme: basic
  type: http
slug: plangrid-authentication
source_filename: plangrid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://developer.plangrid.com/reference/authentication\ndocs: https://developer.plangrid.com/reference/authentication\nsummary:\n  types: [oauth2, http]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode, implicit]\nschemes:\n- name: OAuth2\n  type: oauth2\n  description: >-\n    OAuth 2.0 for authenticating and authorizing PlanGrid users on behalf of an application.\n    Applications must be registered with PlanGrid (contact developers@plangrid.com) with an\n    application name, logo, and list of redirect URIs. Access tokens are sent as\n    \"Authorization: Bearer <access_token>\".\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://io.plangrid.com/oauth/authorize\n    tokenUrl: https://io.plangrid.com/oauth/token\n    refresh: true\n  - flow: implicit\n    authorizationUrl: https://io.plangrid.com/oauth/authorize\n  scopes: [write:projects, read:profile]\n- name: ApiKeyBasic\n  type: http\n \
  \ scheme: basic\n  in: header\n  description: >-\n    HTTP Basic authentication where the API key is sent as the username and the password is left\n    blank (e.g. curl -u API_KEY:). 401 is returned when the API key is missing, 403 when the key\n    is invalid or deactivated.\nheaders:\n  accept: 'application/vnd.plangrid+json; version=1'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plangrid/refs/heads/main/authentication/plangrid-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Enterprise
- Construction
- Construction Technology
- Project Management
- Field Reports
- Documents
- RFIs
- REST API
- Autodesk
---
