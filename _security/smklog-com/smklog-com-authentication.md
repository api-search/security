---
anonymous_access: true
api_key_in: []
api_specs:
- filename: smklog-com-openapi.yml
  format: yaml
  label: SMKlog Quote API
  slug: smklog-quote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smklog-com/refs/heads/main/openapi/smklog-com-openapi.yml
auth_types:
- none
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Smklog Com Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: SMKlog secures its APIs with none and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: SMKlog
provider_slug: smklog-com
scheme_count: 2
schemes:
- applies_to:
  - getParcelQuote
  - createPaymentSession
  - getCheckoutStatus
  - status
  - MCP tools/list + tools/call
  - A2A message/send
  name: anonymous
  note: '"The API works without credentials: rate quotes and payment sessions are open, rate limited per client per hour." (auth.md). The protected-resource document on the API host states authorization_required false.'
  type: none
- bearer: 'Authorization: Bearer smk_at_... on POST /quote'
  failure: 401 invalid_token on an expired or revoked token; "the request is never silently downgraded to anonymous limits, so failures are loud"
  flow: clientCredentials
  issuer: https://quote-api.smklog.com
  name: SMKlog client_credentials
  purpose: '"Credentials exist for one reason — an agent whose legitimate traffic outgrows the anonymous limits gets its own hourly bucket at its own size." Not identity, not authorization for payment.'
  registration: manual — email info@smklog.com with what you are building and the expected volume; the secret is shown once
  scopes:
  - quote
  sources:
  - https://smklog.com/auth.md
  - https://quote-api.smklog.com/.well-known/oauth-authorization-server
  tokenUrl: https://quote-api.smklog.com/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  token_lifetime: one hour
  type: oauth2
slug: smklog-com-authentication
source_filename: smklog-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\ndocs: https://smklog.com/auth.md\nsource: >-\n  https://smklog.com/auth.md (saved verbatim as authentication/smklog-com-auth.md), the RFC 8414 / RFC 9728\n  metadata on both hosts (well-known/), the MCP server card authentication block, and the OpenAPI, which declares\n  no securitySchemes at all — 0-working/derive-authentication.py therefore produced no profile and this file is\n  hand-written from the provider's own documents.\nsummary:\n  types: [none, oauth2]\n  required: false\n  api_key_in: []\n  oauth2_flows: [clientCredentials]\n  default: anonymous — every operation answers without credentials\nschemes:\n- name: anonymous\n  type: none\n  applies_to: [getParcelQuote, createPaymentSession, getCheckoutStatus, status, 'MCP tools/list + tools/call', 'A2A message/send']\n  note: >-\n    \"The API works without credentials: rate quotes and payment sessions are open, rate limited per client per\n    hour.\" (auth.md). The protected-resource\
  \ document on the API host states authorization_required false.\n- name: SMKlog client_credentials\n  type: oauth2\n  flow: clientCredentials\n  issuer: https://quote-api.smklog.com\n  tokenUrl: https://quote-api.smklog.com/oauth/token\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n  scopes: [quote]\n  bearer: 'Authorization: Bearer smk_at_... on POST /quote'\n  token_lifetime: one hour\n  purpose: >-\n    \"Credentials exist for one reason — an agent whose legitimate traffic outgrows the anonymous limits gets its\n    own hourly bucket at its own size.\" Not identity, not authorization for payment.\n  registration: manual — email info@smklog.com with what you are building and the expected volume; the secret is shown once\n  failure: '401 invalid_token on an expired or revoked token; \"the request is never silently downgraded to anonymous limits, so failures are loud\"'\n  sources: [https://smklog.com/auth.md, https://quote-api.smklog.com/.well-known/oauth-authorization-server]\n\
  capabilities:\n  session_id: >-\n    createPaymentSession returns an opaque session_id (pattern ^as_[A-Za-z0-9-]{8,80}$) that is the only thing\n    needed to read that session's status — a bearer-by-knowledge capability, unauthenticated otherwise; the\n    status answer \"never carries names, addresses or emails\".\nobserved:\n- 'POST /oauth/token without credentials -> 401 application/json {\"error\":\"invalid_client\"} (2026-09-19)'\n- 'POST /quote with an empty body, no credentials -> 400 missing_required_fields (the anonymous path works; nothing challenged for auth)'\ndetail: scopes/smklog-com-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smklog-com/refs/heads/main/authentication/smklog-com-authentication.yml
summary_line: none/oauth2 · 2 schemes
tags:
- Company
- Shipping
- Logistics
- Parcel Shipping
- shipping-rates
- Shipping Labels
- E-Commerce
- Agents
- MCP
- A2A
---
