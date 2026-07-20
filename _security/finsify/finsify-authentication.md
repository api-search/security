---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Finsify Authentication
name_suffix: Authentication
oauth_flows: []
overview: Finsify secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Finsify
provider_slug: finsify
scheme_count: 3
schemes:
- description: Partner identifier issued by Finsify. Required on every request.
  in: header
  name: Client-Id
  parameter: Client-Id
  sources:
  - https://docs.finsify.com/
  type: apiKey
- description: Server-side secret for web/backend services. Mutually exclusive with App-secret.
  in: header
  name: Service-secret
  parameter: Service-secret
  sources:
  - https://docs.finsify.com/
  type: apiKey
- description: Mobile-app secret. Mutually exclusive with Service-secret.
  in: header
  name: App-secret
  parameter: App-secret
  sources:
  - https://docs.finsify.com/
  type: apiKey
slug: finsify-authentication
source_filename: finsify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.finsify.com/\ndocs: https://docs.finsify.com/\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    Finsify Hub uses static header credentials issued per partner. Every request\n    carries a Client-Id header identifying the partner, plus exactly one secret:\n    Service-secret for server/web integrations or App-secret for mobile apps.\n    Service-secret and App-secret must never be sent together on the same request.\n    A short-lived connection token (POST /token) then authorizes the end-user's\n    bank login flow; it is a session token, not an OAuth access token.\nschemes:\n  - name: Client-Id\n    type: apiKey\n    in: header\n    parameter: Client-Id\n    description: Partner identifier issued by Finsify. Required on every request.\n    sources: [https://docs.finsify.com/]\n  - name: Service-secret\n    type: apiKey\n    in: header\n    parameter: Service-secret\n   \
  \ description: >-\n      Server-side secret for web/backend services. Mutually exclusive with\n      App-secret.\n    sources: [https://docs.finsify.com/]\n  - name: App-secret\n    type: apiKey\n    in: header\n    parameter: App-secret\n    description: >-\n      Mobile-app secret. Mutually exclusive with Service-secret.\n    sources: [https://docs.finsify.com/]\nconnection_token:\n  operation: POST /token\n  purpose: >-\n    Generates a short-lived connection token used to launch or re-run an\n    end-user's bank login. Reconnect via POST /token/reconnect when a login\n    needs re-authentication.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finsify/refs/heads/main/authentication/finsify-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Financial Services
- Open Banking
- Bank Aggregation
- Financial Data
- Transactions
- Fintech
- Southeast Asia
---
