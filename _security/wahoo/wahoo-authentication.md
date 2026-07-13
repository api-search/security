---
api_key_in: []
api_specs:
- filename: wahoo-cloud-api-openapi.yml
  format: yaml
  label: Wahoo Cloud API
  slug: wahoo-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wahoo/refs/heads/main/openapi/wahoo-cloud-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Wahoo Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Wahoo Fitness secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Wahoo Fitness
provider_slug: wahoo
scheme_count: 1
schemes:
- description: OAuth 2.0 Authorization Code (with PKCE option for public apps). Access tokens are bearer tokens with a 2-hour TTL; refresh tokens are single-use. Starting 2026-01-01, apps are limited to 10 unrevoked access tokens per user.
  flows:
  - authorizationUrl: https://api.wahooligan.com/oauth/authorize
    flow: authorizationCode
    scopes: 12
    tokenUrl: https://api.wahooligan.com/oauth/token
  name: OAuth2
  sources:
  - openapi/wahoo-cloud-api-openapi.yml
  type: oauth2
slug: wahoo-authentication
source_filename: wahoo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wahoo-cloud-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.wahooligan.com/oauth/authorize\n    tokenUrl: https://api.wahooligan.com/oauth/token\n    scopes: 12\n  description: OAuth 2.0 Authorization Code (with PKCE option for public apps). Access tokens\n    are bearer tokens with a 2-hour TTL; refresh tokens are single-use. Starting 2026-01-01,\n    apps are limited to 10 unrevoked access tokens per user.\n  sources:\n  - openapi/wahoo-cloud-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wahoo/refs/heads/main/authentication/wahoo-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Fitness
- Cycling
- Endurance Training
- Bike Computers
- Smart Trainers
- Indoor Cycling
- Heart Rate
- Power Meters
- GPS
- Wearables
- Hardware
- FIT Files
- Webhooks
- OAuth
---
