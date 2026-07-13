---
api_key_in: []
api_specs:
- filename: openapi.yml
  format: yaml
  label: Google Cloud Speech-to-Text API
  slug: google-cloud-speech-to-text-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-speech-to-text/refs/heads/main/openapi/openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Cloud Speech To Text Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Cloud Speech-To-Text secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Cloud Speech-To-Text
provider_slug: google-cloud-speech-to-text
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/openapi.yml
  type: oauth2
slug: google-cloud-speech-to-text-authentication
source_filename: google-cloud-speech-to-text-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 1\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-speech-to-text/refs/heads/main/authentication/google-cloud-speech-to-text-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Audio Processing
- Google Cloud
- Machine Learning
- Speech Recognition
- Transcription
---
