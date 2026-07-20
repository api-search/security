---
api_key_in:
- header
api_specs:
- filename: gameflip-gfapi-openapi.yml
  format: yaml
  label: Gameflip API (GFAPI)
  slug: gameflip-api-gfapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gameflip/refs/heads/main/openapi/gameflip-gfapi-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Gameflip Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gameflip secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gameflip
provider_slug: gameflip
scheme_count: 1
schemes:
- format: GFAPI <apikey>:<totp>
  header_name: Authorization
  in: header
  name: gfapiAuth
  provisioning: API keys and TOTP secrets are created/requested in Gameflip account settings, or issued by Gameflip support. Access is Beta and gated to a limited number of developers.
  sources:
  - openapi/gameflip-gfapi-openapi.yml
  totp:
    algorithm: SHA1
    digits: 6
    period_seconds: 30
  type: apiKey
slug: gameflip-authentication
source_filename: gameflip-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://gameflip.github.io/gfapi/\ndocs: https://gameflip.github.io/gfapi/\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    Custom API-key + TOTP scheme. Every request carries an Authorization header\n    of the form `GFAPI <apikey>:<totp>`, where <totp> is a rotating one-time\n    password derived from the account's TOTP secret. Not OAuth2; there is no\n    scope surface.\nschemes:\n- name: gfapiAuth\n  type: apiKey\n  in: header\n  header_name: Authorization\n  format: 'GFAPI <apikey>:<totp>'\n  totp:\n    algorithm: SHA1\n    digits: 6\n    period_seconds: 30\n  provisioning: >-\n    API keys and TOTP secrets are created/requested in Gameflip account\n    settings, or issued by Gameflip support. Access is Beta and gated to a\n    limited number of developers.\n  sources: [openapi/gameflip-gfapi-openapi.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gameflip/refs/heads/main/authentication/gameflip-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Gaming
- Marketplace
- Digital Goods
- E-Commerce
- Payments
- Wallet
- Listings
- Steam
- Gift Cards
---
