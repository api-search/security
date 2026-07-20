---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Koah Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Koah Labs secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Koah Labs
provider_slug: koah-labs
scheme_count: 1
schemes:
- applies_to: https://app.koah.ai/api
  audience: publisher team accounts only
  format: 'Authorization: Bearer [example key]'
  header: Authorization
  in: header
  issuance: Koah dashboard, Settings > API Tokens
  name: bearerAuth
  notes: '"All API requests require authentication using API keys. You can obtain your API key from your Koah dashboard under the Settings section." The reporting reference adds that only publisher accounts can access the reporting endpoints; advertiser accounts are rejected.'
  scheme: bearer
  source: https://docs.koahlabs.com/api
  type: http
slug: koah-labs-authentication
source_filename: koah-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.koahlabs.com/api\ndocs: https://docs.koahlabs.com/api\nnotes: >-\n  Derived from the published API reference rather than an OpenAPI document —\n  Koah publishes no machine-readable spec. Two distinct credentials exist: an\n  API token for the REST API, and a publisher ID that identifies the app to the\n  client SDKs. The publisher ID is a public client-side identifier, not a secret.\nsummary:\n  types: [http]\n  api_key_in: [header]\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\n  mtls: false\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer [example key]'\n  applies_to: https://app.koah.ai/api\n  issuance: Koah dashboard, Settings > API Tokens\n  audience: publisher team accounts only\n  source: https://docs.koahlabs.com/api\n  notes: >-\n    \"All API requests require authentication using API keys. You can obtain\
  \ your\n    API key from your Koah dashboard under the Settings section.\" The reporting\n    reference adds that only publisher accounts can access the reporting\n    endpoints; advertiser accounts are rejected.\nclient_identifiers:\n- name: publisherId\n  type: public-identifier\n  secret: false\n  applies_to: Ad SDK (JavaScript, React, React Native, Flutter, iOS, Android)\n  issuance: Koah dashboard, Settings > Integration\n  dashboard_url: https://app.koah.ai/publisher/settings?tab=integration\n  transport: query parameter on the web script tag; constructor/config argument on mobile SDKs\n  source: https://docs.koahlabs.com/definitions\n- name: advertiserId\n  type: public-identifier\n  secret: false\n  applies_to: Conversion Tracking pixel\n  dashboard_url: https://app.koah.ai/advertiser/settings?tab=brand\n  source: https://raw.githubusercontent.com/koahlabs/skills/HEAD/skills/koah-integration/SKILL.md\nauth_errors:\n- {status: 401, meaning: Unauthorized — missing or invalid bearer\
  \ token}\n- {status: 403, meaning: Forbidden — token valid but the account type may not access this resource}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/koah-labs/refs/heads/main/authentication/koah-labs-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Ai
- Advertising
- Ad Network
- Monetization
- Conversion Tracking
- SDKs
- Agents
---
