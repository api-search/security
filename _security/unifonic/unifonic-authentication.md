---
api_key_in:
- header
- query
api_specs:
- filename: unifonic-sms-openapi-original.json
  format: json
  label: Unifonic SMS API
  slug: unifonic-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unifonic/refs/heads/main/openapi/unifonic-sms-openapi-original.json
- filename: unifonic-authenticate-openapi-original.json
  format: json
  label: Unifonic Authenticate API
  slug: unifonic-authenticate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unifonic/refs/heads/main/openapi/unifonic-authenticate-openapi-original.json
- filename: unifonic-voice-openapi-original.json
  format: json
  label: Unifonic Voice APIs
  slug: unifonic-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unifonic/refs/heads/main/openapi/unifonic-voice-openapi-original.json
auth_types:
- http-basic
- apiKey
description: 'Provider-wide authentication profile for Unifonic''s public APIs, derived from the securitySchemes declared in the three official OpenAPI documents in this repo''s openapi/ directory and upgraded with the docs Security & Authentication page. Unifonic uses an AppSid/AppsId application credential model rather than OAuth: the SMS NextGen REST API declares HTTP basic authentication and additionally requires an AppSid query parameter on every operation; the Authenticate (OTP) API authenticates with an x-authenticate-app-id header plus an Authorization bearer-token header; the Voice API uses a custom AppsId credential obtained from the Unifonic Console''s Voice Applications tab. HTTPS is recommended for all requests. No oauth2 or openIdConnect security schemes are declared anywhere in the published specs, so there is no OAuth scope surface.'
kind: authentication
layout: security
method: searched
name: Unifonic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Unifonic secures its APIs with http-basic and apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Unifonic
provider_slug: unifonic
scheme_count: 4
schemes:
- name: auth
  note: Declared as the global security requirement of the SMS API. Operations also carry a required AppSid query parameter ("a character string that uniquely identifies your app"); the docs note authentication parameters are base64 encoded (error 459 covers incorrect encoding).
  scheme: basic
  sources:
  - openapi/unifonic-sms-openapi-original.json
  type: http
- in: header
  name: authenticate-app-id
  parameter: x-authenticate-app-id
  sources:
  - openapi/unifonic-authenticate-openapi-original.json
  type: apiKey
- description: Bearer Auth Token
  in: header
  name: Authorization
  parameter: Authorization
  sources:
  - openapi/unifonic-authenticate-openapi-original.json
  type: apiKey
- in: request
  name: AppsId (Voice)
  note: '"This API uses Custom Authentication - AppsId. AppsId is derived from the Unifonic Console''s Voice Application''s tab." The published Voice OpenAPI declares no components.securitySchemes.'
  parameter: AppsId
  sources:
  - https://docs.unifonic.com/articles/api-documentation/security-authentication
  type: custom
slug: unifonic-authentication
source_filename: unifonic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi (unifonic-sms, unifonic-authenticate, unifonic-voice) + docs\ndocs: https://docs.unifonic.com/articles/api-documentation/security-authentication\ndescription: >-\n  Provider-wide authentication profile for Unifonic's public APIs, derived from\n  the securitySchemes declared in the three official OpenAPI documents in this\n  repo's openapi/ directory and upgraded with the docs Security &\n  Authentication page. Unifonic uses an AppSid/AppsId application credential\n  model rather than OAuth: the SMS NextGen REST API declares HTTP basic\n  authentication and additionally requires an AppSid query parameter on every\n  operation; the Authenticate (OTP) API authenticates with an\n  x-authenticate-app-id header plus an Authorization bearer-token header; the\n  Voice API uses a custom AppsId credential obtained from the Unifonic\n  Console's Voice Applications tab. HTTPS is recommended for all requests. No\n  oauth2 or openIdConnect\
  \ security schemes are declared anywhere in the\n  published specs, so there is no OAuth scope surface.\nsummary:\n  types: [http-basic, apiKey]\n  api_key_in: [header, query]\n  oauth2_flows: []\nschemes:\n  - name: auth\n    type: http\n    scheme: basic\n    sources: [openapi/unifonic-sms-openapi-original.json]\n    note: >-\n      Declared as the global security requirement of the SMS API. Operations\n      also carry a required AppSid query parameter (\"a character string that\n      uniquely identifies your app\"); the docs note authentication parameters\n      are base64 encoded (error 459 covers incorrect encoding).\n  - name: authenticate-app-id\n    type: apiKey\n    in: header\n    parameter: x-authenticate-app-id\n    sources: [openapi/unifonic-authenticate-openapi-original.json]\n  - name: Authorization\n    type: apiKey\n    in: header\n    parameter: Authorization\n    description: Bearer Auth Token\n    sources: [openapi/unifonic-authenticate-openapi-original.json]\n  -\
  \ name: AppsId (Voice)\n    type: custom\n    in: request\n    parameter: AppsId\n    sources: [https://docs.unifonic.com/articles/api-documentation/security-authentication]\n    note: >-\n      \"This API uses Custom Authentication - AppsId. AppsId is derived from the\n      Unifonic Console's Voice Application's tab.\" The published Voice OpenAPI\n      declares no components.securitySchemes.\ncredential_provisioning: >-\n  Per the SMS API introduction: \"To start using the API you need to send an\n  email to Unifonic to create Appsid for you.\" Credentials are otherwise\n  managed in the Unifonic cloud console (cloud.unifonic.com).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unifonic/refs/heads/main/authentication/unifonic-authentication.yml
summary_line: http-basic/apiKey · 4 schemes
tags:
- Company
- Enterprise
- CPaaS
- Messaging
- SMS
- WhatsApp
- Voice
- Push Notifications
- OTP
- Customer Engagement
- Saudi Arabia
---
