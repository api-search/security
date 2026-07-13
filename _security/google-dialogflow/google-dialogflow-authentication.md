---
api_key_in: []
api_specs:
- filename: rest
  format: yaml
  label: Dialogflow API
  slug: dialogflow-api
  spec_type: OpenAPI
  url: https://dialogflow.googleapis.com/$discovery/rest?version=v2
- filename: rest
  format: yaml
  label: Dialogflow CX API
  slug: dialogflow-cx-api
  spec_type: OpenAPI
  url: https://dialogflow.googleapis.com/$discovery/rest?version=v3
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Dialogflow Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Dialogflow secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Dialogflow
provider_slug: google-dialogflow
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  sources:
  - openapi/google-dialogflow-openapi.yml
  type: oauth2
slug: google-dialogflow-authentication
source_filename: google-dialogflow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-dialogflow-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 2\n  sources:\n  - openapi/google-dialogflow-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-dialogflow/refs/heads/main/authentication/google-dialogflow-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Artificial Intelligence
- Chatbots
- Conversational AI
- Machine Learning
- Natural Language Processing
- Voice Assistants
---
