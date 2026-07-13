---
api_key_in: []
api_specs:
- filename: strava-openapi.yml
  format: yaml
  label: Strava API
  slug: strava
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/strava/refs/heads/main/openapi/strava-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Strava Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Strava secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Strava
provider_slug: strava
scheme_count: 1
schemes:
- description: OAuth 2.0 Bearer token. Obtain via the authorization code flow at https://www.strava.com/oauth/authorize.
  flows:
  - authorizationUrl: https://www.strava.com/oauth/authorize
    flow: authorizationCode
    scopes: 7
    tokenUrl: https://www.strava.com/oauth/token
  name: stravaBearerAuth
  sources:
  - openapi/strava-openapi.yml
  type: oauth2
slug: strava-authentication
source_filename: strava-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/strava-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: stravaBearerAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.strava.com/oauth/authorize\n    tokenUrl: https://www.strava.com/oauth/token\n    scopes: 7\n  description: OAuth 2.0 Bearer token. Obtain via the authorization code flow at https://www.strava.com/oauth/authorize.\n  sources:\n  - openapi/strava-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/strava/refs/heads/main/authentication/strava-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Cycling
- Fitness
- Fitness Tracking
- Running
- Sports
---
