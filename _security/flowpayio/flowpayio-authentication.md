---
api_key_in:
- header
auth_types:
- oauth2
- apiKey
description: 'Flowpay''s Partner API authenticates with OAuth 2.0 client-credentials, issued by Auth0. Partners exchange a CLIENT_ID/CLIENT_SECRET for a short-lived bearer access token and present it as `Authorization: Bearer <token>` on every request. A PARTNER_CODE identifies the partner and a WEBHOOK_SECRET is used to verify inbound webhook HMAC signatures. The partner-implemented Sales Transactions API additionally accepts a static API key via the `X-API-Key` header. No user-facing OAuth scopes are documented (machine-to-machine client-credentials only).'
kind: authentication
layout: security
method: searched
name: Flowpayio Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: flowpay.io secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: flowpay.io
provider_slug: flowpayio
scheme_count: 2
schemes:
- audience_production: https://api.partner.flowpay.io
  audience_testing: https://api.test.partner.flowpay.io
  credentials:
  - CLIENT_ID
  - CLIENT_SECRET
  - PARTNER_CODE
  flow: clientCredentials
  name: OAuth2ClientCredentials
  presented_as: 'Authorization: Bearer <access_token>'
  scopes: []
  sources:
  - https://developers.flowpay.io/specifications/fully-embedded-api/
  token_url_production: https://flowpay.eu.auth0.com/oauth/token
  token_url_testing: https://flowpay-test.eu.auth0.com/oauth/token
  type: oauth2
- applies_to: Sales Transactions API (partner-implemented data endpoint)
  in: header
  name: ApiKey
  parameter_name: X-API-Key
  sources:
  - https://developers.flowpay.io/specifications/sales-transactions-api/
  type: apiKey
slug: flowpayio-authentication
source_filename: flowpayio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developers.flowpay.io/specifications/fully-embedded-api/\ndocs: https://developers.flowpay.io/specifications/fully-embedded-api/\ndescription: >-\n  Flowpay's Partner API authenticates with OAuth 2.0 client-credentials, issued\n  by Auth0. Partners exchange a CLIENT_ID/CLIENT_SECRET for a short-lived bearer\n  access token and present it as `Authorization: Bearer <token>` on every\n  request. A PARTNER_CODE identifies the partner and a WEBHOOK_SECRET is used to\n  verify inbound webhook HMAC signatures. The partner-implemented Sales\n  Transactions API additionally accepts a static API key via the `X-API-Key`\n  header. No user-facing OAuth scopes are documented (machine-to-machine\n  client-credentials only).\nsummary:\n  types: [oauth2, apiKey]\n  api_key_in: [header]\n  oauth2_flows: [clientCredentials]\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url_production:\
  \ https://flowpay.eu.auth0.com/oauth/token\n  token_url_testing: https://flowpay-test.eu.auth0.com/oauth/token\n  audience_production: https://api.partner.flowpay.io\n  audience_testing: https://api.test.partner.flowpay.io\n  presented_as: 'Authorization: Bearer <access_token>'\n  credentials: [CLIENT_ID, CLIENT_SECRET, PARTNER_CODE]\n  scopes: []\n  sources: [https://developers.flowpay.io/specifications/fully-embedded-api/]\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter_name: X-API-Key\n  applies_to: Sales Transactions API (partner-implemented data endpoint)\n  sources: [https://developers.flowpay.io/specifications/sales-transactions-api/]\nwebhook_verification:\n  mechanism: HMAC-SHA256\n  signature_header: x-flowpay-sig\n  timestamp_header: x-flowpay-ts\n  secret: WEBHOOK_SECRET\n  notes: Timestamp header guards against replay; recompute the HMAC over the raw body and compare.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flowpayio/refs/heads/main/authentication/flowpayio-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Company
- Financing
- Lending
- Embedded Finance
- Fintech
- SME
- Open Banking
- Payments
---
