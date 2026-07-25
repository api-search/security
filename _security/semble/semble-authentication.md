---
api_key_in:
- header
auth_types:
- apiKey
description: 'Semble''s public GraphQL API is authenticated with a bearer-style token passed in a custom "x-token" request header. There is no OAuth 2.0 / OIDC surface and no SMART-on-FHIR; access control is expressed through the role assigned to the token when it is created. Two token kinds exist: long-lived API-access tokens generated in the Semble application (Settings > API Access), each bound to a named role that scopes which queries and mutations it may call; and a short-lived session JWT returned by the signIn mutation, valid for 12 hours.'
kind: authentication
layout: security
method: searched
name: Semble Authentication
name_suffix: Authentication
oauth_flows: []
overview: Semble secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Semble
provider_slug: semble
scheme_count: 1
schemes:
- description: Role-scoped access token. Sent on every GraphQL request as the "x-token" HTTP header. Value is either a long-lived API-access token minted in the Semble app or the 12-hour JWT returned by the signIn mutation.
  in: header
  name: xToken
  parameter_name: x-token
  sources:
  - docs.semble.io/docs/authentication
  type: apiKey
slug: semble-authentication
source_filename: semble-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: https://docs.semble.io/docs/authentication/\ndocs: https://docs.semble.io/docs/authentication/\ndescription: >-\n  Semble's public GraphQL API is authenticated with a bearer-style token passed\n  in a custom \"x-token\" request header. There is no OAuth 2.0 / OIDC surface and\n  no SMART-on-FHIR; access control is expressed through the role assigned to the\n  token when it is created. Two token kinds exist: long-lived API-access tokens\n  generated in the Semble application (Settings > API Access), each bound to a\n  named role that scopes which queries and mutations it may call; and a\n  short-lived session JWT returned by the signIn mutation, valid for 12 hours.\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  api_key_name: x-token\n  oauth2_flows: []\nschemes:\n  - name: xToken\n    type: apiKey\n    in: header\n    parameter_name: x-token\n    description: >-\n      Role-scoped access token. Sent on every GraphQL\
  \ request as the \"x-token\"\n      HTTP header. Value is either a long-lived API-access token minted in the\n      Semble app or the 12-hour JWT returned by the signIn mutation.\n    sources: [docs.semble.io/docs/authentication]\ntoken_kinds:\n  - kind: api-access-token\n    obtained_via: Semble application > Settings > API Access > New (name + role)\n    lifetime: long-lived until revoked\n    scoping: >-\n      Role assigned at creation controls which queries/mutations and which\n      patient/practice data the token can reach.\n  - kind: session-jwt\n    obtained_via: signIn mutation (email + password) -> returns JWT\n    lifetime: 12 hours\n    note: Recommended to sign in at the start of each day.\nnotes: >-\n  Keep tokens secret; they can be revoked in the Semble application. API\n  availability depends on the customer's Semble package/role (contact\n  support@semble.io to enable).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/semble/refs/heads/main/authentication/semble-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Healthcare
- United Kingdom
- EHR
- Practice Management
- GraphQL
- Patient Records
- Scheduling
- e-Prescribing
- Interoperability
- Digital Health
---
