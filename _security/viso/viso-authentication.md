---
api_key_in: []
auth_types:
- oauth2
- session
description: ''
kind: authentication
layout: security
method: searched
name: Viso Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: VISO secures its APIs with oauth2 and session across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: VISO
provider_slug: viso
scheme_count: 2
schemes:
- evidence: now.viso.ai loads https://accounts.google.com/gsi/client
  flow: authorizationCode
  name: GoogleSignIn
  provider: Google Identity Services
  sources:
  - live-probe
  type: oauth2
- applies_to: https://now.viso.ai/api/svc-viso-now/graphql
  evidence: 'anonymous GraphQL `me` query returns 403; credentialed CORS (Access-Control-Allow-Credentials: true)'
  name: SessionCredential
  sources:
  - live-probe
  type: session
slug: viso-authentication
source_filename: viso-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  live probe of https://now.viso.ai (Viso Now app + GraphQL API) and its client\n  bundle; no OpenAPI/GraphQL introspection available (introspection disabled)\nsummary:\n  types: [oauth2, session]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  notes: >-\n    Viso Now signs users in with Google Identity Services\n    (accounts.google.com/gsi/client is loaded by the app) and then carries a\n    session credential to its Apollo GraphQL API. Unauthenticated GraphQL\n    requests to the `me` query return HTTP 403 \"You are not allowed to access\n    this resource\" and CORS is credentialed (Access-Control-Allow-Credentials:\n    true), consistent with cookie/session-bearer auth behind the Google sign-in.\nschemes:\n- name: GoogleSignIn\n  type: oauth2\n  provider: Google Identity Services\n  flow: authorizationCode\n  evidence: 'now.viso.ai loads https://accounts.google.com/gsi/client'\n  sources: [live-probe]\n-\
  \ name: SessionCredential\n  type: session\n  applies_to: https://now.viso.ai/api/svc-viso-now/graphql\n  evidence: >-\n    anonymous GraphQL `me` query returns 403; credentialed CORS\n    (Access-Control-Allow-Credentials: true)\n  sources: [live-probe]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/viso/refs/heads/main/authentication/viso-authentication.yml
summary_line: oauth2/session · 2 schemes
tags:
- Company
- Ai
- Computer Vision
- Machine Learning
- Video Analytics
- Vision Agents
- Edge AI
- GraphQL
- No-Code
---
