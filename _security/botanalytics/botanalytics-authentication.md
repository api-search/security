---
api_key_in: []
api_specs:
- filename: botanalytics-messages-openapi.yml
  format: yaml
  label: Botanalytics Message Ingestion API
  slug: botanalytics-message-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/botanalytics/refs/heads/main/openapi/botanalytics-messages-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Botanalytics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Botanalytics secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Botanalytics
provider_slug: botanalytics
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'A Botanalytics API key is a JSON Web Token (JWT). It is sent as `Authorization: Bearer <token>`. The token carries a `channel` claim that must match the client channel; the SDK validates the JWT shape locally before sending. Missing or invalid tokens return HTTP 401.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/botanalytics-messages-openapi.yml
  - https://github.com/botanalytics/node-sdk/blob/master/core/src/base.js
  type: http
slug: botanalytics-authentication
source_filename: botanalytics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: >-\n  https://docs.beta.botanalytics.co/docs/integration/rest-api/overview +\n  github.com/botanalytics/node-sdk core/src/base.js\ndocs: https://docs.beta.botanalytics.co/docs/integration/rest-api/overview\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  bearer_format: JWT\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: >-\n      A Botanalytics API key is a JSON Web Token (JWT). It is sent as\n      `Authorization: Bearer <token>`. The token carries a `channel` claim that\n      must match the client channel; the SDK validates the JWT shape locally\n      before sending. Missing or invalid tokens return HTTP 401.\n    sources:\n      - openapi/botanalytics-messages-openapi.yml\n      - https://github.com/botanalytics/node-sdk/blob/master/core/src/base.js\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/botanalytics/refs/heads/main/authentication/botanalytics-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Conversational Analytics
- Chatbots
- Voice Assistants
- Bot Analytics
- Analytics
- Natural Language Understanding
- Developer Tools
---
