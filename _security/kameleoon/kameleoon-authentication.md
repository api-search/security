---
api_key_in: []
api_specs:
- filename: kameleoon-openapi.yml
  format: yaml
  label: Kameleoon Automation API
  slug: kameleoon-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kameleoon/refs/heads/main/openapi/kameleoon-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Kameleoon Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Kameleoon secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Kameleoon
provider_slug: kameleoon
scheme_count: 2
schemes:
- bearerFormat: OAuth 2.0 access token
  description: OAuth 2.0 access token obtained from /oauth/token, supplied as a Bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/kameleoon-openapi.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.kameleoon.com/oauth/token
  - authorizationUrl: https://api.kameleoon.com/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://api.kameleoon.com/oauth/token
  name: oauth2
  sources:
  - openapi/kameleoon-openapi.yml
  type: oauth2
slug: kameleoon-authentication
source_filename: kameleoon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kameleoon-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: OAuth 2.0 access token\n  description: OAuth 2.0 access token obtained from /oauth/token, supplied as a Bearer token\n    in the Authorization header.\n  sources:\n  - openapi/kameleoon-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.kameleoon.com/oauth/token\n    scopes: 0\n  - flow: authorizationCode\n    authorizationUrl: https://api.kameleoon.com/oauth/authorize\n    tokenUrl: https://api.kameleoon.com/oauth/token\n    scopes: 0\n  sources:\n  - openapi/kameleoon-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kameleoon/refs/heads/main/authentication/kameleoon-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Experimentation
- AB Testing
- Personalization
- Feature Flags
- AI
---
