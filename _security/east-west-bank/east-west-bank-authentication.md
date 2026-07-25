---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: East West Bank Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: East West Bank secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: East West Bank
provider_slug: east-west-bank
scheme_count: 1
schemes:
- credentials:
    access_token: short-lived bearer access token obtained from the credentials; requests fail with HTTP 401 when the client id/secret do not match the created application or when the access token is invalidated or expired
    client_id: issued per application on application creation
    client_secret: issued per application on application creation
    encoding: base-64 encode the client id and secret in-application (the FAQ recommends encoding in application logic rather than storing a static encoded string)
  flows:
  - flow: clientCredentials
    note: Developers create an "application" (a collection of one or more API resources accessible with a single authentication credential) to obtain a client id and secret. The portal FAQ documents base-64 encoding the client and secret, then exchanging them for an access token that is presented on API calls.
  name: OAuth2
  scheme: standard OAuth 2.0
  sources:
  - https://apiportal.eastwestbank.com/faqs
  type: oauth2
slug: east-west-bank-authentication
source_filename: east-west-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://apiportal.eastwestbank.com/faqs\ndocs: https://apiportal.eastwestbank.com/how-it-works\nnote: >-\n  No OpenAPI/Swagger is publicly downloadable for the Bridge Open Banking program\n  (reference and specs are gated behind portal sign-in and sales onboarding), so this\n  profile is captured from the developer portal's public How It Works and FAQ pages\n  rather than derived from a securityScheme. It reflects what the provider documents.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  api_key_in: []\nschemes:\n- name: OAuth2\n  type: oauth2\n  scheme: standard OAuth 2.0\n  sources:\n  - https://apiportal.eastwestbank.com/faqs\n  flows:\n  - flow: clientCredentials\n    note: >-\n      Developers create an \"application\" (a collection of one or more API resources\n      accessible with a single authentication credential) to obtain a client id and\n      secret. The portal FAQ documents base-64\
  \ encoding the client and secret, then\n      exchanging them for an access token that is presented on API calls.\n  credentials:\n    client_id: issued per application on application creation\n    client_secret: issued per application on application creation\n    encoding: >-\n      base-64 encode the client id and secret in-application (the FAQ recommends\n      encoding in application logic rather than storing a static encoded string)\n    access_token: >-\n      short-lived bearer access token obtained from the credentials; requests fail\n      with HTTP 401 when the client id/secret do not match the created application or\n      when the access token is invalidated or expired\ntroubleshooting:\n- status: 401\n  causes:\n  - client-id and secret not correctly matched against the created application\n  - access token invalidated or expired\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/east-west-bank/refs/heads/main/authentication/east-west-bank-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Financial Services
- Banking
- United States
- Commercial Banking
- Treasury Management
- Cross-Border
- Open Finance
- Data Aggregation
---
