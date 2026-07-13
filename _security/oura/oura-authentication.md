---
api_key_in:
- header
api_specs:
- filename: oura-oura-ring-api-openapi.yml
  format: yaml
  label: Oura Ring API
  slug: oura-ring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oura/refs/heads/main/openapi/oura-oura-ring-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Oura Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Oura Ring secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Oura Ring
provider_slug: oura
scheme_count: 4
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/oura-oura-ring-api-openapi.yml
  type: http
- flows:
  - authorizationUrl: https://cloud.ouraring.com/oauth/authorize
    flow: authorizationCode
    scopes: 8
    tokenUrl: https://api.ouraring.com/oauth/token
  name: OAuth2
  sources:
  - openapi/oura-oura-ring-api-openapi.yml
  type: oauth2
- description: Client ID for webhook subscription endpoints. Must be used together with x-client-secret header.
  in: header
  name: ClientIdAuth
  parameter: x-client-id
  sources:
  - openapi/oura-oura-ring-api-openapi.yml
  type: apiKey
- description: Client Secret for webhook subscription endpoints. Must be used together with x-client-id header.
  in: header
  name: ClientSecretAuth
  parameter: x-client-secret
  sources:
  - openapi/oura-oura-ring-api-openapi.yml
  type: apiKey
slug: oura-authentication
source_filename: oura-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/oura-oura-ring-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/oura-oura-ring-api-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://cloud.ouraring.com/oauth/authorize\n    tokenUrl: https://api.ouraring.com/oauth/token\n    scopes: 8\n  sources:\n  - openapi/oura-oura-ring-api-openapi.yml\n- name: ClientIdAuth\n  type: apiKey\n  in: header\n  parameter: x-client-id\n  description: Client ID for webhook subscription endpoints. Must be used together with x-client-secret\n    header.\n  sources:\n  - openapi/oura-oura-ring-api-openapi.yml\n- name: ClientSecretAuth\n  type: apiKey\n  in: header\n  parameter: x-client-secret\n  description: Client Secret for webhook subscription endpoints.\
  \ Must be used together with\n    x-client-id header.\n  sources:\n  - openapi/oura-oura-ring-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oura/refs/heads/main/authentication/oura-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- Health
- Wearables
- Sleep
- Fitness
- Heart Rate
- Readiness
- Smart Ring
- Biometrics
---
