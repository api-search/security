---
api_key_in: []
api_specs:
- filename: rest
  format: yaml
  label: Android Management API
  slug: android-management-api
  spec_type: OpenAPI
  url: https://androidmanagement.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Google Play Developer API
  slug: google-play-developer-api
  spec_type: OpenAPI
  url: https://androidpublisher.googleapis.com/$discovery/rest?version=v3
- filename: rest
  format: yaml
  label: Firebase Cloud Messaging API
  slug: firebase-cloud-messaging-api
  spec_type: OpenAPI
  url: https://fcm.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Google Play Games Services API
  slug: google-play-games-services-api
  spec_type: OpenAPI
  url: https://www.googleapis.com/discovery/v1/apis/games/v1/rest
- filename: rest
  format: yaml
  label: Android Over the Air API
  slug: android-over-the-air-api
  spec_type: OpenAPI
  url: https://androidovertheair.googleapis.com/$discovery/rest?version=v1
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Android Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Android secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Android
provider_slug: google-android
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  sources:
  - openapi/google-android-openapi.yml
  type: oauth2
slug: google-android-authentication
source_filename: google-android-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-android-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 1\n  sources:\n  - openapi/google-android-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-android/refs/heads/main/authentication/google-android-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Android
- Google
- Mobile Development
- Mobile Operating System
- Open Source
---
