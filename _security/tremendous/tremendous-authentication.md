---
api_key_in: []
api_specs:
- filename: tremendous-api-openapi.yml
  format: yaml
  label: Tremendous API
  slug: tremendous
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tremendous/refs/heads/main/openapi/tremendous-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Tremendous Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Tremendous secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Tremendous
provider_slug: tremendous
scheme_count: 2
schemes:
- description: Bearer token authentication using a Tremendous API key. Generate API keys in your Tremendous dashboard Settings > API.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/tremendous-api-openapi.yml
  type: http
- description: OAuth 2.0 for third-party integrations
  flows:
  - authorizationUrl: https://www.tremendous.com/oauth/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://www.tremendous.com/oauth/token
  name: OAuth2
  sources:
  - openapi/tremendous-api-openapi.yml
  type: oauth2
slug: tremendous-authentication
source_filename: tremendous-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tremendous-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication using a Tremendous API key. Generate API keys in\n    your Tremendous dashboard Settings > API.\n  sources:\n  - openapi/tremendous-api-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.tremendous.com/oauth/authorize\n    tokenUrl: https://www.tremendous.com/oauth/token\n    scopes: 3\n  description: OAuth 2.0 for third-party integrations\n  sources:\n  - openapi/tremendous-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tremendous/refs/heads/main/authentication/tremendous-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Employee Incentives
- Global Payouts
- Incentives
- Market Research
- Payouts
- Rewards
---
