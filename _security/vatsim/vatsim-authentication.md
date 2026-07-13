---
api_key_in:
- header
api_specs:
- filename: openapi.json
  format: json
  label: VATSIM Core API
  slug: vatsim-core-api
  spec_type: OpenAPI
  url: https://api.vatsim.net/v2/openapi.json
- filename: openapi.json
  format: json
  label: VATSIM Data API
  slug: vatsim-data-api
  spec_type: OpenAPI
  url: https://data.vatsim.net/openapi.json
- filename: metar.yaml
  format: yaml
  label: VATSIM METAR API
  slug: vatsim-metar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/metar.yaml
- filename: connect.yaml
  format: yaml
  label: VATSIM Connect API
  slug: vatsim-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/connect.yaml
- filename: slurper.yaml
  format: yaml
  label: VATSIM Slurper API
  slug: vatsim-slurper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/slurper.yaml
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
