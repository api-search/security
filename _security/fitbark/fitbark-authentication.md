---
api_key_in: []
api_specs:
- filename: fitbark-openapi.yml
  format: yaml
  label: FitBark API v2
  slug: fitbark-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbark/refs/heads/main/openapi/fitbark-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Fitbark Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: FitBark secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: FitBark
provider_slug: fitbark
scheme_count: 2
schemes:
- description: OAuth 2.0 user access token (Bearer) obtained from /oauth/token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/fitbark-openapi.yml
  type: http
- description: FitBark OAuth 2.0
  flows:
  - authorizationUrl: https://app.fitbark.com/oauth/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://app.fitbark.com/oauth/token
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://app.fitbark.com/oauth/token
  name: oauth2
  sources:
  - openapi/fitbark-openapi.yml
  type: oauth2
slug: fitbark-authentication
source_filename: fitbark-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/fitbark-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 user access token (Bearer) obtained from /oauth/token\n  sources:\n  - openapi/fitbark-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.fitbark.com/oauth/authorize\n    tokenUrl: https://app.fitbark.com/oauth/token\n    scopes: 1\n  - flow: clientCredentials\n    tokenUrl: https://app.fitbark.com/oauth/token\n    scopes: 1\n  description: FitBark OAuth 2.0\n  sources:\n  - openapi/fitbark-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fitbark/refs/heads/main/authentication/fitbark-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Dogs
- Pets
- Wearables
- Activity Tracking
- Health
- IoT
- Fitness
---
