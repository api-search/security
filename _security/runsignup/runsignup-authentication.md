---
api_key_in:
- query
api_specs:
- filename: runsignup-openapi.yml
  format: yaml
  label: RunSignup API
  slug: runsignup
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runsignup/refs/heads/main/openapi/runsignup-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Runsignup Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: RunSignup secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: RunSignup
provider_slug: runsignup
scheme_count: 2
schemes:
- description: OAuth 2.0 authentication (preferred)
  flows:
  - authorizationUrl: https://runsignup.com/OAuth/Authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://runsignup.com/OAuth/Token
  name: OAuth2
  sources:
  - openapi/runsignup-openapi.yml
  type: oauth2
- description: Permanent API key for affiliates, partners, and timers. Pass api_key and api_secret as query parameters.
  in: query
  name: apiKeyAuth
  parameter: api_key
  sources:
  - openapi/runsignup-openapi.yml
  type: apiKey
slug: runsignup-authentication
source_filename: runsignup-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/runsignup-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://runsignup.com/OAuth/Authorize\n    tokenUrl: https://runsignup.com/OAuth/Token\n    scopes: 2\n  description: OAuth 2.0 authentication (preferred)\n  sources:\n  - openapi/runsignup-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Permanent API key for affiliates, partners, and timers. Pass api_key and api_secret\n    as query parameters.\n  sources:\n  - openapi/runsignup-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runsignup/refs/heads/main/authentication/runsignup-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Race Registration
- Event Management
- Running
- Sports
- Fitness
- Timing
- Fundraising
---
