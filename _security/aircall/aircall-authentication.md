---
api_key_in: []
api_specs:
- filename: aircall-webhooks-asyncapi.yml
  format: yaml
  label: Aircall Webhooks API
  slug: aircall-webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/aircall/refs/heads/main/asyncapi/aircall-webhooks-asyncapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Aircall Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Aircall secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Aircall
provider_slug: aircall
scheme_count: 2
schemes:
- description: Aircall customer authentication using api_id (username) and api_token (password) sent as HTTP Basic auth.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/aircall-openapi.yml
  type: http
- description: OAuth 2.0 authorization code flow for Aircall Marketplace technology partners.
  flows:
  - authorizationUrl: https://auth.aircall.io/oauth/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://auth.aircall.io/oauth/token
  name: OAuth2
  sources:
  - openapi/aircall-openapi.yml
  type: oauth2
slug: aircall-authentication
source_filename: aircall-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aircall-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: Aircall customer authentication using api_id (username) and api_token (password)\n    sent as HTTP Basic auth.\n  sources:\n  - openapi/aircall-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.aircall.io/oauth/authorize\n    tokenUrl: https://auth.aircall.io/oauth/token\n    scopes: 1\n  description: OAuth 2.0 authorization code flow for Aircall Marketplace technology partners.\n  sources:\n  - openapi/aircall-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aircall/refs/heads/main/authentication/aircall-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Communications
- Voice
- Cloud Phone
- CRM
- Sales
---
