---
api_key_in: []
api_specs:
- filename: pitney-bowes-openapi.yml
  format: yaml
  label: Pitney Bowes APIs
  slug: pitney-bowes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pitney-bowes/refs/heads/main/openapi/pitney-bowes-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Pitney Bowes Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Pitney Bowes secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Pitney Bowes
provider_slug: pitney-bowes
scheme_count: 2
schemes:
- description: Used only on /oauth/token to obtain an access token.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/pitney-bowes-openapi.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://shipping-api.pitneybowes.com/oauth/token
  name: oauth2
  sources:
  - openapi/pitney-bowes-openapi.yml
  type: oauth2
slug: pitney-bowes-authentication
source_filename: pitney-bowes-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pitney-bowes-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Used only on /oauth/token to obtain an access token.\n  sources:\n  - openapi/pitney-bowes-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://shipping-api.pitneybowes.com/oauth/token\n    scopes: 0\n  sources:\n  - openapi/pitney-bowes-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pitney-bowes/refs/heads/main/authentication/pitney-bowes-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Mailing
- Shipping
- Fortune 1000
---
