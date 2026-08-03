---
api_key_in:
- header
auth_types:
- none
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Huel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Huel secures its APIs with none and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Huel
provider_slug: huel
scheme_count: 3
schemes:
- description: 'Public read endpoints require no credential. Verified 2026-08-01: GET /about.json, /site.json, /categories.json, /latest.json and /users/{username}.json all returned HTTP 200 application/json without authentication.'
  evidence:
  - http_status: 200
    url: https://discourse.huel.com/about.json
  - http_status: 200
    url: https://discourse.huel.com/site.json
  - http_status: 200
    url: https://discourse.huel.com/categories.json
  - http_status: 200
    url: https://discourse.huel.com/latest.json
  - http_status: 200
    url: https://discourse.huel.com/users/system.json
  name: anonymous
  type: none
  verified: true
- description: Discourse admin-issued API keys are sent as the Api-Key header together with an Api-Username header naming the acting user. Keys are minted only from the forum admin panel; Huel publishes no self-service issuance path, so this tier is not available to third-party developers.
  in: header
  name: discourse-api-key
  names:
  - Api-Key
  - Api-Username
  note: Documented Discourse platform behaviour (docs.discourse.org), not observed on this host - admin endpoints such as /admin/users/list/active.json return 404 to anonymous callers rather than a 401/403 challenge.
  self_service: false
  type: apiKey
  verified: false
- description: Discourse's per-user API key flow for third-party clients, negotiated through /user-api-key/new with an RSA public key. Also a Discourse platform capability rather than a Huel-published one.
  in: header
  name: discourse-user-api-key
  names:
  - User-Api-Key
  self_service: false
  type: apiKey
  verified: false
slug: huel-authentication
source_filename: huel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: https://discourse.huel.com/site.json\ndocs: https://docs.discourse.org/\nsummary:\n  types: [none, apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  first_party_auth_docs: false\nnotes: >-\n  Huel operates no developer programme and publishes no authentication\n  documentation, because it exposes no first-party API. This profile describes the\n  authentication model of the one anonymously callable machine-readable surface found\n  on a Huel-controlled host: the Discourse platform REST API served by the Huel US\n  customer forum at discourse.huel.com (Discourse 2026.8.0). The auth model is\n  Discourse's, documented upstream at docs.discourse.org, not something Huel authored.\n  There is no OpenAPI in this repo, so nothing here was derived from securitySchemes;\n  the anonymous tier below was verified by live probe and the keyed tier is the\n  documented Discourse contract.\nschemes:\n- name: anonymous\n  type: none\n \
  \ description: >-\n    Public read endpoints require no credential. Verified 2026-08-01: GET\n    /about.json, /site.json, /categories.json, /latest.json and /users/{username}.json\n    all returned HTTP 200 application/json without authentication.\n  verified: true\n  evidence:\n  - {url: 'https://discourse.huel.com/about.json', http_status: 200}\n  - {url: 'https://discourse.huel.com/site.json', http_status: 200}\n  - {url: 'https://discourse.huel.com/categories.json', http_status: 200}\n  - {url: 'https://discourse.huel.com/latest.json', http_status: 200}\n  - {url: 'https://discourse.huel.com/users/system.json', http_status: 200}\n- name: discourse-api-key\n  type: apiKey\n  in: header\n  names: [Api-Key, Api-Username]\n  description: >-\n    Discourse admin-issued API keys are sent as the Api-Key header together with an\n    Api-Username header naming the acting user. Keys are minted only from the forum\n    admin panel; Huel publishes no self-service issuance path, so this tier is\
  \ not\n    available to third-party developers.\n  self_service: false\n  verified: false\n  note: >-\n    Documented Discourse platform behaviour (docs.discourse.org), not observed on this\n    host - admin endpoints such as /admin/users/list/active.json return 404 to\n    anonymous callers rather than a 401/403 challenge.\n- name: discourse-user-api-key\n  type: apiKey\n  in: header\n  names: [User-Api-Key]\n  description: >-\n    Discourse's per-user API key flow for third-party clients, negotiated through\n    /user-api-key/new with an RSA public key. Also a Discourse platform capability\n    rather than a Huel-published one.\n  self_service: false\n  verified: false\nend_user_identity:\n  description: >-\n    Forum sign-in for humans (not an API credential path). site.json advertises two\n    social auth providers alongside local accounts.\n  providers: [facebook, twitter/x, local]\n  login_required: false\nabsent:\n- {scheme: oauth2, reason: no OAuth authorization server found on\
  \ any Huel host}\n- {scheme: openIdConnect, reason: '/.well-known/openid-configuration returned 404'}\n- {scheme: mutualTLS, reason: not published}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/huel/refs/heads/main/authentication/huel-authentication.yml
summary_line: none/apiKey · 3 schemes
tags:
- Company
- Food and Beverage
- Nutrition
- Consumer Packaged Goods
- Direct to Consumer
- E-Commerce
- Subscription Commerce
- Health and Wellness
- Retail
- United Kingdom
---
