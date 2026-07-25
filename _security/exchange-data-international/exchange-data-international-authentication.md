---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Exchange Data International Authentication
name_suffix: Authentication
oauth_flows: []
overview: Exchange Data International secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Exchange Data International
provider_slug: exchange-data-international
scheme_count: 1
schemes:
- description: Production license key sent in the Authorization header. Per the API FAQ, "Upon registration the Prod License key will be enabled from day 1" - users register on the developer portal and use the production key when integrating. All 24 API products on the shared api3.exchange-data.com base require it; access to each product is gated by per-product subscription.
  evidence:
  - probe: GET https://api3.exchange-data.com/GetLatestEODPrices?MIC=USCOMP&format=json (no Authorization header)
    result: 'HTTP 401 {"error": "Authorization field missing"}'
  - probe: 'GET with header Authorization: Bearer notatoken'
    result: 'HTTP 403 {"error": "Access to this API has been disallowed"}'
  in: header
  name: LicenseKey
  parameter: Authorization
  type: apiKey
slug: exchange-data-international-authentication
source_filename: exchange-data-international-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: https://developer.exchange-data.com/p/api-faq\ndocs: https://developer.exchange-data.com/p/api-faq\nnote: EDI publishes no OpenAPI, so this profile is captured from the developer portal\n  docs, the API FAQ, and live probes of the api3.exchange-data.com host on 2026-07-22.\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: LicenseKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Production license key sent in the Authorization header. Per the API\n    FAQ, \"Upon registration the Prod License key will be enabled from day 1\" - users\n    register on the developer portal and use the production key when integrating.\n    All 24 API products on the shared api3.exchange-data.com base require it; access\n    to each product is gated by per-product subscription.\n  evidence:\n  - probe: GET https://api3.exchange-data.com/GetLatestEODPrices?MIC=USCOMP&format=json\n\
  \      (no Authorization header)\n    result: 'HTTP 401 {\"error\": \"Authorization field missing\"}'\n  - probe: 'GET with header Authorization: Bearer notatoken'\n    result: 'HTTP 403 {\"error\": \"Access to this API has been disallowed\"}'\nonboarding:\n  register: https://developer.exchange-data.com/register\n  notes: Self-serve registration on the EDI Developer portal grants an account, access\n    to the API Playground, and a production license key from day 1; individual API\n    products require a subscription.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exchange-data-international/refs/heads/main/authentication/exchange-data-international-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Financial
- Market Data
- Corporate Actions
- Reference Data
- End of Day Pricing
- Fixed Income
- Derivatives
- Economic Data
- Stocks
- Exchange
---
