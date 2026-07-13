---
api_key_in: []
api_specs:
- filename: openapi.yml
  format: yaml
  label: Pixelfed REST API
  slug: pixelfed-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Pixelfed Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Pixelfed secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Pixelfed
provider_slug: pixelfed
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://{instance}/oauth/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://{instance}/oauth/token
  name: OAuth2
  sources:
  - openapi/openapi.yml
  type: oauth2
- bearerFormat: OAuth2
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/openapi.yml
  type: http
slug: pixelfed-authentication
source_filename: pixelfed-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{instance}/oauth/authorize\n    tokenUrl: https://{instance}/oauth/token\n    scopes: 4\n  sources:\n  - openapi/openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: OAuth2\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/authentication/pixelfed-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Fediverse
- ActivityPub
- Photo Sharing
- Social Media
- Open Source
- Decentralized
- Mastodon Compatible
- Federation
---
