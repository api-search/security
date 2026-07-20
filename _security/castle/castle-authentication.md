---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Castle Authentication
name_suffix: Authentication
oauth_flows: []
overview: Castle secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Castle
provider_slug: castle
scheme_count: 1
schemes:
- description: 'Backend requests authenticate with HTTP Basic authentication. The API Secret is supplied as the HTTP Basic password (username left empty), i.e. `Authorization: Basic base64(":<API_SECRET>")`. The secret is configured server-side via the CASTLE_API_SECRET environment variable in the official SDKs. Client-side calls use a separate publishable App ID with the browser/ mobile SDK to generate a short-lived request token; the secret is never exposed to the client.'
  name: apiSecretBasic
  scheme: basic
  sources:
  - https://docs.castle.io/docs/integration-guide
  type: http
slug: castle-authentication
source_filename: castle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.castle.io/docs/integration-guide + https://docs.castle.io/docs/enterprise-using-events-api\ndocs: https://docs.castle.io/docs/integration-guide\nsummary:\n  types:\n  - http\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: apiSecretBasic\n  type: http\n  scheme: basic\n  description: >-\n    Backend requests authenticate with HTTP Basic authentication. The API Secret\n    is supplied as the HTTP Basic password (username left empty), i.e.\n    `Authorization: Basic base64(\":<API_SECRET>\")`. The secret is configured\n    server-side via the CASTLE_API_SECRET environment variable in the official\n    SDKs. Client-side calls use a separate publishable App ID with the browser/\n    mobile SDK to generate a short-lived request token; the secret is never\n    exposed to the client.\n  sources:\n  - https://docs.castle.io/docs/integration-guide\nnotes:\n- Base URL is https://api.castle.io.\n- The Events\
  \ API (enterprise) uses the same HTTP Basic [example key] scheme.\n- No OAuth2 / OpenID Connect surface is documented; therefore no scopes/ artifact.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/castle/refs/heads/main/authentication/castle-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Security
- Fraud Prevention
- Bot Detection
- Device Fingerprinting
- Account Takeover
- Risk Scoring
- Identity
---
