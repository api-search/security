---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Reebelo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Reebelo declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Reebelo
provider_slug: reebelo
scheme_count: 2
schemes:
- applies_to:
  - GET sockets/offers
  - POST sockets/offers/update
  - GET sockets/orders
  - PUT sockets/orders/track
  - PUT sockets/orders/imei
  description: 'Reebelo-issued static API key. Sent on every sockets/* request alongside content-type: application/json. Documented request header example is {"content-type":"application/json", "x-api-key":"xxxxxx"}.'
  expiry: not documented
  id: x-api-key
  in: header
  name: x-api-key
  provisioning: Issued by Reebelo. Not self-service — a vendor receives the key from their Reebelo account manager by email, and integration partners are instructed to email Reebelo support to request it.
  rotation: not documented
  type: apiKey
- applies_to:
  - POST cobalt/orders/{orderNumber}/invoices/upload-url
  description: Bearer token used on the seller invoice presigned-upload endpoint. Documented header example is {"content-type":"application/json", "Authorization":"Bearer xxxxxx"}.
  id: bearer
  in: header
  name: Authorization
  provisioning: not documented
  scheme: bearer
  type: http
slug: reebelo-authentication
source_filename: reebelo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://cobalt.reebelo.com/documentation/custom-api\ndocs: https://cobalt.reebelo.com/documentation/custom-api\napi: Reebelo Vendor Integration API (Cobalt)\nbase_urls:\n  production: https://a.reebelo.com\n  staging: https://a.reebelo.blue\nsummary: >-\n  Reebelo's vendor API uses a single static API key passed in an x-api-key request\n  header. The key is issued by Reebelo — the documentation states it is \"to be\n  provided by Reebelo\" and third-party integrators are told to email Reebelo support\n  to request their token. There is no self-service key provisioning, no OAuth, and no\n  published scope model. One endpoint (seller invoice upload) instead takes an\n  Authorization: Bearer credential.\nschemes:\n- id: x-api-key\n  type: apiKey\n  in: header\n  name: x-api-key\n  description: >-\n    Reebelo-issued static API key. Sent on every sockets/* request alongside\n    content-type: application/json. Documented request\
  \ header example is\n    {\"content-type\":\"application/json\", \"x-api-key\":\"xxxxxx\"}.\n  applies_to:\n  - GET sockets/offers\n  - POST sockets/offers/update\n  - GET sockets/orders\n  - PUT sockets/orders/track\n  - PUT sockets/orders/imei\n  provisioning: >-\n    Issued by Reebelo. Not self-service — a vendor receives the key from their Reebelo\n    account manager by email, and integration partners are instructed to email Reebelo\n    support to request it.\n  rotation: not documented\n  expiry: not documented\n- id: bearer\n  type: http\n  scheme: bearer\n  in: header\n  name: Authorization\n  description: >-\n    Bearer token used on the seller invoice presigned-upload endpoint. Documented\n    header example is {\"content-type\":\"application/json\", \"Authorization\":\"Bearer xxxxxx\"}.\n  applies_to:\n  - POST cobalt/orders/{orderNumber}/invoices/upload-url\n  provisioning: not documented\noauth2: false\nopenid_connect: false\nmutual_tls: false\nscopes: none published\nnotes:\n\
  - >-\n  The two credential styles are not reconciled in the documentation: the offer/order\n  surface is x-api-key and the invoice-upload surface is Authorization: Bearer. An\n  integrator must hold both to cover the full flow.\n- >-\n  a.reebelo.com is an AWS API Gateway. Unauthenticated requests return HTTP 403 with\n  {\"message\":\"Forbidden\"} at the edge, or {\"message\":\"Missing Authentication Token\"}\n  for an unmatched route — neither is an RFC 7235 challenge, so there is no\n  WWW-Authenticate header to discover the scheme from.\n- >-\n  Cobalt back-office (human) accounts are separate from API keys and are subject to a\n  90-day password expiry policy stated in the Cobalt login flow.\nevidence:\n- url: https://cobalt.reebelo.com/documentation/custom-api\n  status: 200\n  note: Documentation content is served inside the SPA JavaScript bundle (/assets/index.8b57822b.js)\n- url: https://a.reebelo.com/\n  status: 403\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reebelo/refs/heads/main/authentication/reebelo-authentication.yml
summary_line: 2 schemes
tags:
- Refurbished Electronics
- Marketplace
- E-Commerce
- Consumer Electronics
- Reverse Logistics
- Circular Economy
- Retail
- Inventory
- Order
- Seller Integration
---
