---
api_key_in:
- query
auth_types:
- apiKey
- oauth2
- bearer
- serviceAccount
- idToken
description: ''
kind: authentication
layout: security
method: searched
name: Firebase Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- serviceAccount
overview: Firebase secures its APIs with apiKey, oauth2, bearer, serviceAccount, and idToken across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and serviceAccount flow(s).
provider_name: Firebase
provider_slug: firebase
scheme_count: 5
schemes:
- in: query
  name: apiKey
  note: Firebase Web API key identifies the project on public REST endpoints (Identity Toolkit, RTDB, Remote Config). Not a secret by itself — access is governed by Security Rules and App Check.
  parameter: key
  type: apiKey
- authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
  name: oauth2
  note: Google-hosted management/data REST APIs (Firebase Management, Firestore, FCM v1) authenticate with Google OAuth 2.0 bearer access tokens. See scopes/firebase-scopes.yml.
  tokenUrl: https://oauth2.googleapis.com/token
  type: oauth2
- flow: serviceAccount
  name: serviceAccount
  note: Admin SDK and server-to-server access use a Google service-account key (GOOGLE_APPLICATION_CREDENTIALS) exchanged for an OAuth access token.
  type: oauth2
- bearerFormat: JWT
  name: firebaseIdToken
  note: Firebase Authentication issues client ID tokens (JWTs) verified server-side by the Admin SDK; issuer https://securetoken.google.com/<project-id>.
  type: bearer
- in: header
  name: appCheck
  note: App Check attestation token asserting the request comes from an authentic app instance; complements user auth, does not replace it.
  parameter: X-Firebase-AppCheck
  type: apiKey
slug: firebase-authentication
source_filename: firebase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: >-\n  https://firebase.google.com/docs/auth,\n  https://firebase.google.com/docs/projects/api/reference/rest,\n  https://cloud.google.com/docs/authentication\nsummary:\n  types: [apiKey, oauth2, bearer, serviceAccount, idToken]\n  api_key_in: [query]\n  oauth2_flows: [authorizationCode, serviceAccount]\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: key\n  note: >-\n    Firebase Web API key identifies the project on public REST endpoints\n    (Identity Toolkit, RTDB, Remote Config). Not a secret by itself — access is\n    governed by Security Rules and App Check.\n- name: oauth2\n  type: oauth2\n  note: >-\n    Google-hosted management/data REST APIs (Firebase Management, Firestore,\n    FCM v1) authenticate with Google OAuth 2.0 bearer access tokens. See\n    scopes/firebase-scopes.yml.\n  authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n  tokenUrl: https://oauth2.googleapis.com/token\n\
  - name: serviceAccount\n  type: oauth2\n  flow: serviceAccount\n  note: >-\n    Admin SDK and server-to-server access use a Google service-account key\n    (GOOGLE_APPLICATION_CREDENTIALS) exchanged for an OAuth access token.\n- name: firebaseIdToken\n  type: bearer\n  bearerFormat: JWT\n  note: >-\n    Firebase Authentication issues client ID tokens (JWTs) verified server-side\n    by the Admin SDK; issuer https://securetoken.google.com/<project-id>.\n- name: appCheck\n  type: apiKey\n  in: header\n  parameter: X-Firebase-AppCheck\n  note: >-\n    App Check attestation token asserting the request comes from an authentic\n    app instance; complements user auth, does not replace it.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/firebase/refs/heads/main/authentication/firebase-authentication.yml
summary_line: apiKey/oauth2/bearer/serviceAccount/idToken · 5 schemes
tags:
- Company
- Backend as a Service
- Application Development
- Mobile
- Web
- Authentication
- Database
- Cloud Functions
- Messaging
- Google
---
