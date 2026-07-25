---
api_key_in:
- header
api_specs:
- filename: vatsim-events-api-openapi.yml
  format: yaml
  label: VATSIM Events API
  slug: vatsim-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-events-api-openapi.yml
- filename: vatsim-metar-api-openapi.yml
  format: yaml
  label: VATSIM METAR API
  slug: vatsim-metar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-metar-api-openapi.yml
- filename: vatsim-airport-info-api-openapi.yml
  format: yaml
  label: VATSIM Airport info API
  slug: vatsim-airport-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-airport-info-api-openapi.yml
- filename: vatsim-atc-api-openapi.yml
  format: yaml
  label: VATSIM atc API
  slug: vatsim-atc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-atc-api-openapi.yml
- filename: vatsim-audio-api-openapi.yml
  format: yaml
  label: VATSIM Audio API
  slug: vatsim-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-audio-api-openapi.yml
- filename: vatsim-community-api-openapi.yml
  format: yaml
  label: VATSIM community API
  slug: vatsim-community-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-community-api-openapi.yml
- filename: vatsim-data-feed-api-openapi.yml
  format: yaml
  label: VATSIM Data feed API
  slug: vatsim-data-feed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-data-feed-api-openapi.yml
- filename: vatsim-event-info-api-openapi.yml
  format: yaml
  label: VATSIM Event info API
  slug: vatsim-event-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-event-info-api-openapi.yml
- filename: vatsim-events-api-openapi.yml
  format: yaml
  label: VATSIM Events API
  slug: vatsim-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-events-api-openapi.yml
- filename: vatsim-members-api-openapi.yml
  format: yaml
  label: VATSIM members API
  slug: vatsim-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-members-api-openapi.yml
- filename: vatsim-metar-api-openapi.yml
  format: yaml
  label: VATSIM METAR API
  slug: vatsim-metar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-metar-api-openapi.yml
- filename: vatsim-oauth2-api-openapi.yml
  format: yaml
  label: VATSIM OAuth2 API
  slug: vatsim-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-oauth2-api-openapi.yml
- filename: vatsim-orgs-api-openapi.yml
  format: yaml
  label: VATSIM orgs API
  slug: vatsim-orgs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-orgs-api-openapi.yml
- filename: vatsim-servers-api-openapi.yml
  format: yaml
  label: VATSIM Servers API
  slug: vatsim-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-servers-api-openapi.yml
- filename: vatsim-user-api-openapi.yml
  format: yaml
  label: VATSIM User API
  slug: vatsim-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-user-api-openapi.yml
- filename: vatsim-users-api-openapi.yml
  format: yaml
  label: VATSIM Users API
  slug: vatsim-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-users-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Vatsim Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: VATSIM secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: VATSIM
provider_slug: vatsim
scheme_count: 3
schemes:
- flows:
  - authorizationUrl: /oauth/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: /oauth/token
  name: connect
  sources:
  - openapi/connect.yaml
  type: oauth2
- description: Preferred method of authentication for APIv2. Use your APIv2 key here.
  in: header
  name: APIKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/core-api.json
  type: apiKey
- description: 'Preserved for backwards compatibility with API v1, **not recommended** for new integrations.


    The same API key used in the `X-API-Key` header should be used here, but prefixed with `Token `.'
  in: header
  name: LegacyAuth
  parameter: Authorization
  sources:
  - openapi/core-api.json
  type: apiKey
slug: vatsim-authentication
source_filename: vatsim-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/connect.yaml, openapi/core-api.json\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: connect\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /oauth/authorize\n    tokenUrl: /oauth/token\n    scopes: 4\n  sources:\n  - openapi/connect.yaml\n- name: APIKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Preferred method of authentication for APIv2. Use your APIv2 key here.\n  sources:\n  - openapi/core-api.json\n- name: LegacyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    Preserved for backwards compatibility with API v1, **not recommended** for new integrations.\n\n    The same API key used in the `X-API-Key` header should be used here, but prefixed with `Token `.\n  sources:\n  - openapi/core-api.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/authentication/vatsim-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Aviation
- Flight Simulation
- Air Traffic Control
- Real-Time Data
- Community
---
