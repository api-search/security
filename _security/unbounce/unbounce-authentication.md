---
api_key_in: []
api_specs:
- filename: unbounce-openapi.yml
  format: yaml
  label: Unbounce REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbounce/refs/heads/main/openapi/unbounce-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Unbounce Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Unbounce secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Unbounce
provider_slug: unbounce
scheme_count: 2
schemes:
- description: HTTP Basic auth using the Unbounce API key as the username.
  name: apiKeyAuth
  scheme: basic
  sources:
  - openapi/unbounce-openapi.yml
  type: http
- description: OAuth 2.0 Authorization Code (granted case-by-case by Unbounce).
  flows:
  - authorizationUrl: https://api.unbounce.com/oauth/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://api.unbounce.com/oauth/token
  name: oauth2
  sources:
  - openapi/unbounce-openapi.yml
  type: oauth2
slug: unbounce-authentication
source_filename: unbounce-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/unbounce-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: apiKeyAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic auth using the Unbounce API key as the username.\n  sources:\n  - openapi/unbounce-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.unbounce.com/oauth/authorize\n    tokenUrl: https://api.unbounce.com/oauth/token\n    scopes: 2\n  description: OAuth 2.0 Authorization Code (granted case-by-case by Unbounce).\n  sources:\n  - openapi/unbounce-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unbounce/refs/heads/main/authentication/unbounce-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Landing Pages
- Conversion Rate Optimization
- Marketing
- A/B Testing
- Lead Generation
- Marketing Automation
---
