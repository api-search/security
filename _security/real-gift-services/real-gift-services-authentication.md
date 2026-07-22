---
api_key_in: []
auth_types: []
description: 'RealGifts authenticates API and SDK calls with an API key. The public developer snippet initializes the browser SDK with an API key (RealGifts.init({ api_key: ''YOUR_API_KEY'' })). No OAuth or OpenID Connect flow is advertised on the public developer surface. The full auth reference lives in the gated documentation portal.'
kind: authentication
layout: security
method: searched
name: Real Gift Services Authentication
name_suffix: Authentication
oauth_flows: []
overview: Real Gift Services declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Real Gift Services
provider_slug: real-gift-services
scheme_count: 1
schemes:
- description: 'API key issued to the integrating platform/vendor account. Passed to the SDK via RealGifts.init({ api_key: ''...'' }) for browser integrations and used to authenticate REST API and webhook requests. Header/parameter name and key prefix are documented in the gated portal and not captured here.'
  evidence: 'Homepage developer snippet — "Initialize with your API key" / RealGifts.init({ api_key: ''YOUR_API_KEY'' }).'
  id: api_key
  in: header
  official: true
  parameter: unknown
  type: apiKey
slug: real-gift-services-authentication
source_filename: real-gift-services-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://www.getrealgifts.com/documentation\ntype: Authentication\nprovider: Real Gift Services\napi: RealGifts API\ndocs: https://www.getrealgifts.com/documentation\ndescription: >-\n  RealGifts authenticates API and SDK calls with an API key. The public\n  developer snippet initializes the browser SDK with an API key\n  (RealGifts.init({ api_key: 'YOUR_API_KEY' })). No OAuth or OpenID Connect flow\n  is advertised on the public developer surface. The full auth reference lives in\n  the gated documentation portal.\nschemes:\n- id: api_key\n  type: apiKey\n  official: true\n  in: header\n  parameter: unknown\n  description: >-\n    API key issued to the integrating platform/vendor account. Passed to the\n    SDK via RealGifts.init({ api_key: '...' }) for browser integrations and used\n    to authenticate REST API and webhook requests. Header/parameter name and\n    key prefix are documented in the gated portal and not captured\
  \ here.\n  evidence: >-\n    Homepage developer snippet — \"Initialize with your API key\" /\n    RealGifts.init({ api_key: 'YOUR_API_KEY' }).\nnotes: >-\n  Vendor vs. standard account types exist (signup?account_type=vendor); scope of\n  key permissions per account type is not documented publicly.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/real-gift-services/refs/heads/main/authentication/real-gift-services-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Gifting
- Gift Cards
- Rewards
- Loyalty
- E-Commerce
- Commerce
- Embedded Commerce
- API
- SDKs
- Webhooks
---
