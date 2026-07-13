---
api_key_in: []
api_specs:
- filename: envato-openapi.yml
  format: yaml
  label: Envato Market API
  slug: market
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envato/refs/heads/main/openapi/envato-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Envato Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Envato secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Envato
provider_slug: envato
scheme_count: 2
schemes:
- bearerFormat: Personal Token
  description: 'Envato personal token issued from build.envato.com. Sent as `Authorization: Bearer <token>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/envato-openapi.yml
  type: http
- flows:
  - authorizationUrl: https://api.envato.com/authorization
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://api.envato.com/token
  name: oauth2
  sources:
  - openapi/envato-openapi.yml
  type: oauth2
slug: envato-authentication
source_filename: envato-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/envato-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Personal Token\n  description: 'Envato personal token issued from build.envato.com. Sent as `Authorization:\n    Bearer <token>`.'\n  sources:\n  - openapi/envato-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.envato.com/authorization\n    tokenUrl: https://api.envato.com/token\n    scopes: 1\n  sources:\n  - openapi/envato-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/envato/refs/heads/main/authentication/envato-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Stock Media
- Marketplace
- Themes
- Audio
- Video
- Graphics
- Subscription
---
