---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: bot-butcher-classification-api-openapi.yml
  format: yaml
  label: Bot Butcher Classification API
  slug: bot-butcher-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bot-butcher/refs/heads/main/openapi/bot-butcher-classification-api-openapi.yml
auth_types:
- apiKey
description: Authentication profile for the Bot Butcher Classification API. A single static API key sent in the x-api-key request header authenticates every operation. There is no OAuth, no OIDC, no bearer token, no mTLS and no signed-request scheme. Read from the provider's published API reference (HTTP 200, fetched 2026-09-04) and cross-checked against the provider's public Postman collection, whose collection-level auth block is apikey / header / x-api-key.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Bot Butcher Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bot Butcher secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bot Butcher
provider_slug: bot-butcher
scheme_count: 1
schemes:
- applies_to:
  - classifyMessage
  - getMessage
  description: 'Required on every request. Documented as "x-api-key: (Required) API key to authenticate the request." The provider''s Postman collection describes API_KEY as "Each Form has its own key", so a key is scoped to a single contact form rather than to the whole account.'
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  required: true
  sources:
  - https://botbutcher.com/documentation
  - openapi/bot-butcher-classification-api-openapi.yml
  - collections/bot-butcher-api-published.postman_collection.json
  type: apiKey
slug: bot-butcher-authentication
source_filename: bot-butcher-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: https://botbutcher.com/documentation\ndocs: https://botbutcher.com/documentation\ndescription: >-\n  Authentication profile for the Bot Butcher Classification API. A single static API key sent in\n  the x-api-key request header authenticates every operation. There is no OAuth, no OIDC, no\n  bearer token, no mTLS and no signed-request scheme. Read from the provider's published API\n  reference (HTTP 200, fetched 2026-09-04) and cross-checked against the provider's public\n  Postman collection, whose collection-level auth block is apikey / header / x-api-key.\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - header\n  oauth: false\n  oidc: false\n  mtls: false\n  anonymous_access: false\nschemes:\n  - name: ApiKeyAuth\n    type: apiKey\n    in: header\n    parameter: x-api-key\n    required: true\n    applies_to:\n      - classifyMessage\n      - getMessage\n    description: >-\n      Required on every request. Documented\
  \ as \"x-api-key: (Required) API key to authenticate the\n      request.\" The provider's Postman collection describes API_KEY as \"Each Form has its own key\",\n      so a key is scoped to a single contact form rather than to the whole account.\n    sources:\n      - https://botbutcher.com/documentation\n      - openapi/bot-butcher-classification-api-openapi.yml\n      - collections/bot-butcher-api-published.postman_collection.json\nkey_management:\n  issuance:\n    url: https://botbutcher.com/get-started\n    flow: >-\n      Self-serve. Create an account with first name, last name and a verified email address, or\n      continue with Google or GitHub, and accept the terms; the key is issued from the account.\n    verification: Email verification is required.\n  rotation:\n    documented: false\n    note: No key rotation, expiry, revocation or scoping procedure is documented.\n  scopes:\n    documented: false\n    note: >-\n      No OAuth scopes and no permission model are published.\
  \ Keys are per-form, which is the only\n      granularity the provider describes.\n  transport:\n    tls_required: true\n    note: The documented base URL is https://api.botbutcher.com; no plaintext endpoint is published.\nfailure_modes:\n  - status: 401\n    meaning: Unauthorized — returned when authentication fails.\n    source: https://botbutcher.com/documentation\n  - status: 400\n    meaning: Malformed request — returned when a required header (including x-api-key) is missing.\n    source: https://botbutcher.com/documentation\ngaps:\n  - No documented key rotation or revocation procedure.\n  - No expiry or lifetime is stated for an issued key.\n  - No scope or least-privilege model beyond one key per form.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bot-butcher/refs/heads/main/authentication/bot-butcher-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Bots
- Spam Detection
- Contact Forms
- AI Classification
- Security
---
