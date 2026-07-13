---
api_key_in:
- header
api_specs:
- filename: rest-api-spec
  format: yaml
  label: Figma REST API
  slug: figma-api
  spec_type: OpenAPI
  url: https://github.com/figma/rest-api-spec
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Wireframes Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Wireframes secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Wireframes
provider_slug: wireframes
scheme_count: 2
schemes:
- description: Personal Access Token authentication for Figma REST API
  in: header
  name: personalAccessToken
  parameter: X-Figma-Token
  sources:
  - openapi/wireframes-openapi.yml
  type: apiKey
- description: OAuth 2.0 authentication for registered applications
  flows:
  - authorizationUrl: https://www.figma.com/oauth
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://api.figma.com/v1/oauth/token
  name: oauth2
  sources:
  - openapi/wireframes-openapi.yml
  type: oauth2
slug: wireframes-authentication
source_filename: wireframes-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wireframes-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: personalAccessToken\n  type: apiKey\n  in: header\n  parameter: X-Figma-Token\n  description: Personal Access Token authentication for Figma REST API\n  sources:\n  - openapi/wireframes-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.figma.com/oauth\n    tokenUrl: https://api.figma.com/v1/oauth/token\n    scopes: 2\n  description: OAuth 2.0 authentication for registered applications\n  sources:\n  - openapi/wireframes-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wireframes/refs/heads/main/authentication/wireframes-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Design
- Figma
- Prototyping
- UI Design
- UX
- Wireframing
---
