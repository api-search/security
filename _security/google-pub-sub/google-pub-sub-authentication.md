---
api_key_in: []
api_specs:
- filename: google-pub-sub-openapi.yml
  format: yaml
  label: Google Pub/Sub
  slug: google-pub-sub
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-pub-sub/refs/heads/main/openapi/google-pub-sub-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Pub Sub Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Pub/Sub secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Pub/Sub
provider_slug: google-pub-sub
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/google-pub-sub-openapi.yml
  type: oauth2
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/google-pub-sub-openapi.yml
  type: http
slug: google-pub-sub-authentication
source_filename: google-pub-sub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-pub-sub-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 2\n  sources:\n  - openapi/google-pub-sub-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/google-pub-sub-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-pub-sub/refs/heads/main/authentication/google-pub-sub-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Cloud
- Event-Driven
- Google Cloud
- Messaging
- Pub/Sub
- Streaming
---
