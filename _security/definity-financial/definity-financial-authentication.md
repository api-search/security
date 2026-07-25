---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Definity Financial Authentication
name_suffix: Authentication
oauth_flows: []
overview: Definity Financial declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Definity Financial
provider_slug: definity-financial
scheme_count: 0
schemes: []
slug: definity-financial-authentication
source_filename: definity-financial-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: >-\n  Live probes of api.definity.com, www.definityfinancial.com, www.economical.com,\n  www.sonnet.ca and broker.economical.com, plus CSIO's certification register\npublished: false\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    Definity Financial publishes no authentication documentation and no machine-readable\n    security scheme. There is no OpenAPI, so there is nothing to derive from. This file is\n    an honest posture record, not a derived scheme list.\nschemes: []\nposture:\n  audience: partner-only\n  self_serve_signup: false\n  public_credentials: false\n  gateway:\n    host: api.definity.com\n    reachable: true\n    documented: false\n    note: >-\n      Resolves behind an Imperva edge (45.60.75.50, 45.60.135.50) and answers HTTP 404 with\n      content-length 0 to every anonymous path, including /.well-known/openid-configuration\n      and /.well-known/oauth-authorization-server.\
  \ A production/partner gateway with zero\n      public discovery surface.\n  broker_channel:\n    host: broker.economical.com\n    reachable: true\n    documented: false\n    note: >-\n      Docebo SaaS learning management system (CNAME economical.docebosaas.com) serving broker\n      training courseware behind a sign-in wall. A login wall, not a developer portal and not\n      an authorization server.\n  consumer_channel:\n    host: www.sonnet.ca\n    login: https://www.sonnet.ca/account-log-in\n    note: Policyholder web account for the direct-to-consumer Sonnet brand. Not an API credential surface.\nattested_model:\n  standard: CSIO API Security Standards\n  certified: true\n  certified_on: '2024-11-27'\n  body: Centre for Study of Insurance Operations (CSIO)\n  description: >-\n    Although Definity documents no authentication scheme publicly, it IS certified against\n    CSIO's API Security Standards, which define a standard authentication and authorization\n    API model for insurer-to-Broker-Management-System\
  \ connectivity. The Standards were\n    produced by CSIO's INNOTECH Advisory Committee and its API Security Working Group, address\n    OAuth 2.1 security concerns, and require certified members to confirm prevention of 16\n    OAuth security concerns and 18 API endpoint concerns. This is third-party attestation of\n    an OAuth-family model on the gated broker channel — it is NOT a first-party contract, and\n    the specific grant types, token endpoints and scopes remain unpublished.\n  sources:\n  - https://csio.com/news/csio-congratulates-definity-financial-corporation-achieving-api-security-standards\n  - https://csio.com/csio-certification/certified-members\nprobes:\n- url: https://api.definity.com/.well-known/openid-configuration\n  status: 404\n- url: https://api.definity.com/.well-known/oauth-authorization-server\n  status: 404\n- url: https://api.definity.com/.well-known/oauth-protected-resource\n  status: 404\n- url: https://www.sonnet.ca/.well-known/openid-configuration\n  status:\
  \ 404\n- url: https://www.definityfinancial.com/.well-known/openid-configuration\n  status: 200\n  note: Body is the eleven-byte string \"Invalid key\" — not OpenID Provider metadata.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/definity-financial/refs/heads/main/authentication/definity-financial-authentication.yml
summary_line: 0 schemes
tags:
- Insurance
- Canada
- Property and Casualty
- Carrier
- Underwriting
- Claims
- Broker
- Pet Insurance
- Direct to Consumer
- Partner Gated
- CSIO
- Insurtech
---
