---
api_key_in:
- body
auth_types:
- apiKey
- customHash
description: ''
kind: authentication
layout: security
method: searched
name: Easebuzz Authentication
name_suffix: Authentication
oauth_flows: []
overview: Easebuzz secures its APIs with apiKey and customHash across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Easebuzz
provider_slug: easebuzz
scheme_count: 2
schemes:
- description: Merchant key issued in the Easebuzz dashboard, sent with each request.
  in: body
  name: merchantKey
  parameter: key
  sources:
  - https://docs.easebuzz.in/
  type: apiKey
- algorithm: SHA-512
  description: SHA-512 hash over an ordered, pipe-delimited payload plus the merchant salt, proving request integrity and authenticity. The salt is a shared secret and is never sent on the wire.
  in: body
  name: requestHash
  parameter: hash
  sources:
  - https://docs.easebuzz.in/
  type: customHash
slug: easebuzz-authentication
source_filename: easebuzz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.easebuzz.in/\nsummary:\n  types:\n  - apiKey\n  - customHash\n  api_key_in:\n  - body\n  oauth2_flows: []\nnotes: >-\n  Easebuzz REST APIs (Payment Gateway and Wire Payouts) authenticate each request with a\n  merchant \"key\" issued in the dashboard and a per-request integrity \"hash\". The hash is a\n  SHA-512 digest computed over a pipe-delimited, ordered concatenation of the request\n  parameters bracketed by the merchant \"salt\" (a shared secret that is never transmitted).\n  The response is verified the same way (reverse-order hash). There is no OAuth 2.0 / OIDC\n  surface. Test and live use separate key/salt pairs and separate hosts.\nschemes:\n- name: merchantKey\n  type: apiKey\n  in: body\n  parameter: key\n  description: Merchant key issued in the Easebuzz dashboard, sent with each request.\n  sources:\n  - https://docs.easebuzz.in/\n- name: requestHash\n  type: customHash\n  algorithm: SHA-512\n  in:\
  \ body\n  parameter: hash\n  description: >-\n    SHA-512 hash over an ordered, pipe-delimited payload plus the merchant salt, proving\n    request integrity and authenticity. The salt is a shared secret and is never sent on\n    the wire.\n  sources:\n  - https://docs.easebuzz.in/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/easebuzz/refs/heads/main/authentication/easebuzz-authentication.yml
summary_line: apiKey/customHash · 2 schemes
tags:
- Company
- Fintech
- Payments
- Payment Gateway
- Payouts
- Banking
- India
- UPI
- Subscriptions
- SDK
---
