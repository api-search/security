---
api_key_in: []
api_specs:
- filename: google-pub-sub-publish-api-openapi.yml
  format: yaml
  label: Google Pub/Sub Publish API
  slug: google-pub-sub-publish-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-pub-sub/refs/heads/main/openapi/google-pub-sub-publish-api-openapi.yml
- filename: google-pub-sub-schemas-api-openapi.yml
  format: yaml
  label: Google Pub/Sub Schemas API
  slug: google-pub-sub-schemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-pub-sub/refs/heads/main/openapi/google-pub-sub-schemas-api-openapi.yml
- filename: google-pub-sub-snapshots-api-openapi.yml
  format: yaml
  label: Google Pub/Sub Snapshots API
  slug: google-pub-sub-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-pub-sub/refs/heads/main/openapi/google-pub-sub-snapshots-api-openapi.yml
- filename: google-pub-sub-subscribe-api-openapi.yml
  format: yaml
  label: Google Pub/Sub Subscribe API
  slug: google-pub-sub-subscribe-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-pub-sub/refs/heads/main/openapi/google-pub-sub-subscribe-api-openapi.yml
- filename: google-pub-sub-subscriptions-api-openapi.yml
  format: yaml
  label: Google Pub/Sub Subscriptions API
  slug: google-pub-sub-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-pub-sub/refs/heads/main/openapi/google-pub-sub-subscriptions-api-openapi.yml
- filename: google-pub-sub-topics-api-openapi.yml
  format: yaml
  label: Google Pub/Sub Topics API
  slug: google-pub-sub-topics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-pub-sub/refs/heads/main/openapi/google-pub-sub-topics-api-openapi.yml
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
