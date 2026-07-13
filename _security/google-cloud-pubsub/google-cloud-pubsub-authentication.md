---
api_key_in: []
api_specs:
- filename: google-cloud-pubsub-openapi.yml
  format: yaml
  label: Google Cloud Pub/Sub API
  slug: google-cloud-pubsub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-pubsub/refs/heads/main/openapi/google-cloud-pubsub-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Cloud Pubsub Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Cloud Pub/Sub secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Cloud Pub/Sub
provider_slug: google-cloud-pubsub
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/google-cloud-pubsub-openapi.yml
  type: oauth2
slug: google-cloud-pubsub-authentication
source_filename: google-cloud-pubsub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-cloud-pubsub-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 2\n  sources:\n  - openapi/google-cloud-pubsub-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-pubsub/refs/heads/main/authentication/google-cloud-pubsub-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Event-Driven
- Google Cloud
- Messaging
- Pub/Sub
---
