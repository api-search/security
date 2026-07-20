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
method: searched
name: Google Android Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- jwtBearer (service account)
overview: Google Android secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and jwtBearer (service account) flow(s).
provider_name: Google Android
provider_slug: google-android
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
    use: interactive user consent
  - flow: serviceAccount
    mechanism: JWT bearer (RFC 7523) exchanged at token endpoint; optional domain-wide delegation
    tokenUrl: https://oauth2.googleapis.com/token
    use: server-to-server (recommended for enterprise/EMM automation)
  name: OAuth2
  sources:
  - openapi/google-android-openapi.yml
  type: oauth2
slug: google-android-authentication
source_filename: google-android-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: Google Discovery documents + https://developers.google.com/android/management/authentication\ndocs:\n  - https://developers.google.com/android/management/authentication\n  - https://developers.google.com/identity/protocols/oauth2\n  - https://developers.google.com/identity/protocols/oauth2/service-account\nsummary:\n  types:\n    - oauth2\n  oauth2_flows:\n    - authorizationCode\n    - jwtBearer (service account)\n  identity_host: https://accounts.google.com\nschemes:\n  - name: OAuth2\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n        tokenUrl: https://oauth2.googleapis.com/token\n        use: interactive user consent\n      - flow: serviceAccount\n        mechanism: JWT bearer (RFC 7523) exchanged at token endpoint; optional domain-wide delegation\n        tokenUrl: https://oauth2.googleapis.com/token\n        use: server-to-server\
  \ (recommended for enterprise/EMM automation)\n    sources:\n      - openapi/google-android-openapi.yml\nnotes: >-\n  Every API in this repo authenticates with Google OAuth 2.0 access tokens (Bearer)\n  scoped per Discovery document (see scopes/). Server integrations use Google service\n  accounts (JWT bearer). Firebase Cloud Messaging additionally supports the Firebase\n  Admin SDK credential flow. Play Integrity verdicts are additionally protected by\n  Google-managed keys. No API keys or basic auth are used for these management APIs.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-android/refs/heads/main/authentication/google-android-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Android
- Google
- Mobile Development
- Mobile Operating System
- Open Source
---
