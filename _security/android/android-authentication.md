---
api_key_in: []
api_specs:
- filename: google-play-developer-api.yml
  format: yaml
  label: Google Play Developer APIs
  slug: google-play-developer-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/android/refs/heads/main/openapi/google-play-developer-api.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Android Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Android secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Android
provider_slug: android
scheme_count: 1
schemes:
- description: OAuth 2.0 authentication for accessing the Google Play Developer API. Requires a service account with appropriate permissions in the Google Play Console.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/google-play-developer-api.yml
  type: oauth2
slug: android-authentication
source_filename: android-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-play-developer-api.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 1\n  description: OAuth 2.0 authentication for accessing the Google Play Developer API. Requires\n    a service account with appropriate permissions in the Google Play Console.\n  sources:\n  - openapi/google-play-developer-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/android/refs/heads/main/authentication/android-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- AI
- Android
- Automotive
- Google
- Machine Learning
- Mobile Development
- SDK
- TV
- Wearables
---
