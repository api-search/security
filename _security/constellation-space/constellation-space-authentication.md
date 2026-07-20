---
api_key_in: []
api_specs:
- filename: constellation-space-openapi.yml
  format: yaml
  label: ConstellationOS API
  slug: constellationos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constellation-space/refs/heads/main/openapi/constellation-space-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Constellation Space Authentication
name_suffix: Authentication
oauth_flows: []
overview: Constellation Space secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Constellation Space
provider_slug: constellation-space
scheme_count: 1
schemes:
- env_var: CONSTELLATION_API_TOKEN
  format: 'Authorization: Bearer <token>'
  header: Authorization
  lifecycle:
    created_in: Settings -> API (console)
    revocable: instant (Settings -> API); in-flight requests fail immediately after revocation propagates
    shown_once: true
    validated: on every API request
  name: bearerAuth
  scheme: bearer
  scopes:
  - topology:read
  - telemetry:write
  - predictions:run
  sources:
  - openapi/constellation-space-openapi.yml
  token_prefixes:
    non_production: cos_dev_
    production: cos_live_
  type: http
slug: constellation-space-authentication
source_filename: constellation-space-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.constellation.space/connect/api-tokens\ndocs: https://docs.constellation.space/connect/api-tokens\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    Static, scoped API tokens presented as HTTP bearer credentials. Not an\n    OAuth2 authorization-code flow — tokens are minted in the console, not\n    granted via an authorization server. Scopes are attached to the token at\n    creation time.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  header: Authorization\n  format: 'Authorization: Bearer <token>'\n  token_prefixes:\n    production: cos_live_\n    non_production: cos_dev_\n  env_var: CONSTELLATION_API_TOKEN\n  lifecycle:\n    created_in: Settings -> API (console)\n    shown_once: true\n    revocable: instant (Settings -> API); in-flight requests fail immediately after revocation propagates\n    validated: on every API request\n\
  \  scopes:\n  - topology:read\n  - telemetry:write\n  - predictions:run\n  sources:\n  - openapi/constellation-space-openapi.yml\nexample: |\n  export CONSTELLATION_API_TOKEN=cos_live_your_token_here\n  curl -sS -H \"Authorization: Bearer $CONSTELLATION_API_TOKEN\" \\\n    \"https://api.constellation.space/api/v1/topology/\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/constellation-space/refs/heads/main/authentication/constellation-space-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Satellites
- Space
- Telemetry
- Machine Learning
- Fleet Operations
- Ground Segment
- Predictions
---
