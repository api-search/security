---
api_key_in: []
api_specs:
- filename: swagger.yaml
  format: yaml
  label: Polar AccessLink API
  slug: polar-accesslink-api
  spec_type: OpenAPI
  url: https://www.polar.com/accesslink-api/swagger.yaml
- filename: swagger.yaml
  format: yaml
  label: Polar TeamPro API
  slug: polar-teampro-api
  spec_type: OpenAPI
  url: https://www.polar.com/teampro-api/swagger.yaml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Polar Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Polar secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Polar
provider_slug: polar
scheme_count: 2
schemes:
- name: Basic
  scheme: basic
  sources:
  - openapi/polar-accesslink-api-openapi.yml
  type: http
- flows:
  - authorizationUrl: https://flow.polar.com/oauth2/authorization
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://polarremote.com/v2/oauth2/token
  name: OAuth2
  sources:
  - openapi/polar-accesslink-api-openapi.yml
  - openapi/polar-teampro-api-openapi.yml
  type: oauth2
slug: polar-authentication
source_filename: polar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/polar-accesslink-api-openapi.yml, openapi/polar-teampro-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: Basic\n  type: http\n  scheme: basic\n  sources:\n  - openapi/polar-accesslink-api-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://flow.polar.com/oauth2/authorization\n    tokenUrl: https://polarremote.com/v2/oauth2/token\n    scopes: 1\n  sources:\n  - openapi/polar-accesslink-api-openapi.yml\n  - openapi/polar-teampro-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/authentication/polar-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Fitness
- Health
- Wearables
- Heart Rate
- Sports
- Training
- Sleep
- Activity Tracking
- Sensors
- Bluetooth
---
