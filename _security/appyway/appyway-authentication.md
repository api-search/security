---
api_key_in:
- header
api_specs:
- filename: appyway-availability-realtime-api-openapi.yml
  format: yaml
  label: AppyWay Availability RealTime API
  slug: appyway-availability-realtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appyway/refs/heads/main/openapi/appyway-availability-realtime-api-openapi.yml
- filename: appyway-traffic-data-api-openapi.yml
  format: yaml
  label: AppyWay Traffic Data API
  slug: appyway-traffic-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appyway/refs/heads/main/openapi/appyway-traffic-data-api-openapi.yml
- filename: appyway-explorer-api-openapi.yml
  format: yaml
  label: AppyWay Explorer API
  slug: appyway-explorer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appyway/refs/heads/main/openapi/appyway-explorer-api-openapi.yml
- filename: appyway-platform-api-openapi.yml
  format: yaml
  label: AppyWay Platform API
  slug: appyway-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appyway/refs/heads/main/openapi/appyway-platform-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Appyway Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: AppyWay secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: AppyWay
provider_slug: appyway
scheme_count: 2
schemes:
- in: header
  name: apiKey
  parameter: API-KEY
  sources:
  - openapi/appyway-availability-realtime-api-openapi.yml
  - openapi/appyway-explorer-api-openapi.yml
  - openapi/appyway-platform-api-openapi.yml
  - openapi/appyway-traffic-data-api-openapi.yml
  - openapi/availability-realtime-api-openapi.yml
  - openapi/explorer-api-openapi.yml
  - openapi/traffic-data-api-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: https://auth.appyway.com/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://auth.appyway.com/oauth/token
  name: oAuth2
  sources:
  - openapi/appyway-availability-realtime-api-openapi.yml
  - openapi/appyway-explorer-api-openapi.yml
  - openapi/appyway-platform-api-openapi.yml
  - openapi/appyway-traffic-data-api-openapi.yml
  - openapi/availability-realtime-api-openapi.yml
  - openapi/explorer-api-openapi.yml
  - openapi/traffic-data-api-openapi.yml
  type: oauth2
slug: appyway-authentication
source_filename: appyway-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/appyway-availability-realtime-api-openapi.yml, openapi/appyway-explorer-api-openapi.yml,\n  openapi/appyway-platform-api-openapi.yml, openapi/appyway-traffic-data-api-openapi.yml, openapi/availability-realtime-api-openapi.yml,\n  openapi/explorer-api-openapi.yml, openapi/traffic-data-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: API-KEY\n  sources:\n  - openapi/appyway-availability-realtime-api-openapi.yml\n  - openapi/appyway-explorer-api-openapi.yml\n  - openapi/appyway-platform-api-openapi.yml\n  - openapi/appyway-traffic-data-api-openapi.yml\n  - openapi/availability-realtime-api-openapi.yml\n  - openapi/explorer-api-openapi.yml\n  - openapi/traffic-data-api-openapi.yml\n- name: oAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.appyway.com/authorize\n\
  \    tokenUrl: https://auth.appyway.com/oauth/token\n    scopes: 0\n  sources:\n  - openapi/appyway-availability-realtime-api-openapi.yml\n  - openapi/appyway-explorer-api-openapi.yml\n  - openapi/appyway-platform-api-openapi.yml\n  - openapi/appyway-traffic-data-api-openapi.yml\n  - openapi/availability-realtime-api-openapi.yml\n  - openapi/explorer-api-openapi.yml\n  - openapi/traffic-data-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appyway/refs/heads/main/authentication/appyway-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Parking
- Traffic
- Urban Mobility
- Smart Cities
- EV Charging
---
