---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Admob Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: AdMob secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: AdMob
provider_slug: admob
scheme_count: 1
schemes:
- authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
  flow: authorizationCode
  name: GoogleOAuth2
  scopes:
  - https://www.googleapis.com/auth/admob.readonly
  - https://www.googleapis.com/auth/admob.report
  sources:
  - docs
  tokenUrl: https://oauth2.googleapis.com/token
  type: oauth2
slug: admob-authentication
source_filename: admob-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://developers.google.com/admob/api/v1/auth\ndocs: https://developers.google.com/admob/api/v1/auth\nsummary:\n  types: [oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\nnotes: >-\n  All AdMob API calls must be authorized through Google OAuth 2.0. Applications\n  obtain user consent, receive an authorization code, exchange it for access and\n  refresh tokens, and call admob.googleapis.com with a Bearer access token.\n  Credentials are created in the Google API Console (OAuth client ID). Service\n  accounts are not supported for the AdMob API; a user must authorize access.\nschemes:\n- name: GoogleOAuth2\n  type: oauth2\n  flow: authorizationCode\n  authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n  tokenUrl: https://oauth2.googleapis.com/token\n  scopes:\n  - https://www.googleapis.com/auth/admob.readonly\n  - https://www.googleapis.com/auth/admob.report\n  sources: [docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/admob/refs/heads/main/authentication/admob-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Advertising
- Mobile
- Monetization
- Ads
- Google
- Reporting
- Mediation
- AdTech
---
