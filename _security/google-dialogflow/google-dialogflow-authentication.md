---
anonymous_access: false
api_key_in: []
api_specs:
- filename: google-dialogflow-projects-api-openapi.yml
  format: yaml
  label: Google Dialogflow Projects API
  slug: google-dialogflow-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-dialogflow/openapi/google-dialogflow-projects-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Google Dialogflow Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Dialogflow secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Dialogflow
provider_slug: google-dialogflow
scheme_count: 2
schemes:
- description: Google OAuth 2.0. Scopes are declared per operation in the Discovery Document.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  sources:
  - openapi/google-dialogflow-cx-v3-openapi.yml
  - openapi/google-dialogflow-es-v2-openapi.yml
  type: oauth2
- description: 'Google OAuth 2.0 access token or service-account-minted bearer token, sent as Authorization: Bearer <token>.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/google-dialogflow-cx-v3-openapi.yml
  - openapi/google-dialogflow-es-v2-openapi.yml
  type: http
slug: google-dialogflow-authentication
source_filename: google-dialogflow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: derived\nsource: openapi/google-dialogflow-cx-v3-openapi.yml, openapi/google-dialogflow-es-v2-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 2\n  description: Google OAuth 2.0. Scopes are declared per operation in the Discovery Document.\n  sources:\n  - openapi/google-dialogflow-cx-v3-openapi.yml\n  - openapi/google-dialogflow-es-v2-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'Google OAuth 2.0 access token or service-account-minted bearer token, sent as\n    Authorization: Bearer <token>.'\n  sources:\n  - openapi/google-dialogflow-cx-v3-openapi.yml\n  - openapi/google-dialogflow-es-v2-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-dialogflow/authentication/google-dialogflow-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Agents
- Artificial Intelligence
- Chatbots
- Conversational AI
- Google Cloud
- Machine Learning
- Natural Language Processing
- Speech Recognition
- Virtual Agents
- Voice Assistant
---
