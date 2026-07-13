---
api_key_in:
- header
api_specs:
- filename: ptc-thingworx-rest-openapi.yml
  format: yaml
  label: PTC ThingWorx REST API
  slug: thingworx-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ptc-thingworx/refs/heads/main/openapi/ptc-thingworx-rest-openapi.yml
- filename: ptc-thingworx-websocket-asyncapi.yml
  format: yaml
  label: PTC ThingWorx WebSocket/AlwaysOn API
  slug: thingworx-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/ptc-thingworx/refs/heads/main/asyncapi/ptc-thingworx-websocket-asyncapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Ptc Thingworx Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: ptc-thingworx secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: ptc-thingworx
provider_slug: ptc-thingworx
scheme_count: 2
schemes:
- description: ThingWorx Application Key for authentication
  in: header
  name: appKey
  parameter: appKey
  sources:
  - openapi/ptc-thingworx-rest-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: https://thingworx.example.com/oauth/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://thingworx.example.com/oauth/token
  name: oauth2
  sources:
  - openapi/ptc-thingworx-rest-openapi.yml
  type: oauth2
slug: ptc-thingworx-authentication
source_filename: ptc-thingworx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ptc-thingworx-rest-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: appKey\n  type: apiKey\n  in: header\n  parameter: appKey\n  description: ThingWorx Application Key for authentication\n  sources:\n  - openapi/ptc-thingworx-rest-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://thingworx.example.com/oauth/authorize\n    tokenUrl: https://thingworx.example.com/oauth/token\n    scopes: 1\n  sources:\n  - openapi/ptc-thingworx-rest-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ptc-thingworx/refs/heads/main/authentication/ptc-thingworx-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags: []
---
