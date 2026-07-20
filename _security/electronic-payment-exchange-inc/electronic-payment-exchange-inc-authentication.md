---
api_key_in: []
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Electronic Payment Exchange Inc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Electronic payment Exchange Inc secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Electronic payment Exchange Inc
provider_slug: electronic-payment-exchange-inc
scheme_count: 2
schemes:
- description: Legacy four-part processing key that identifies the merchant on Browser Post API and Hosted Pay Page transaction requests. Composed of four numeric fields sent with each transaction.
  fields:
  - CUST_NBR
  - MERCH_NBR
  - DBA_NBR
  - TERMINAL_NBR
  in: body
  name: FourPartKey
  source: https://developer.north.com/supplemental-resources/epx-data-dictionary/transaction-request-fields
  type: apiKey
  used_by:
  - Browser Post API
  - Hosted Pay Page
  - Hosted Checkout
- description: HMAC-style request signing for the North EPX Custom Pay REST API. The caller sends an identity header plus a computed signature over the request, provisioned by the North integrations team. Signature computation is documented in the "How To Authenticate" section of the Custom Pay API Integration Guide.
  headers:
  - EPI-Id
  - EPI-Signature
  - EPI-Trace
  in: header
  name: EPISignature
  source: https://developer.north.com/blog/tutorial-nodejs-browser-post-custom-pay-api
  type: apiKey
  used_by:
  - North EPX Custom Pay REST API
slug: electronic-payment-exchange-inc-authentication
source_filename: electronic-payment-exchange-inc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developer.north.com/\ndocs:\n- https://developer.north.com/supplemental-resources/epx-data-dictionary/transaction-request-fields\n- https://developer.north.com/blog/tutorial-nodejs-browser-post-custom-pay-api\n- https://developer.north.com/products/online/epx-hosted-checkout/integration-guide\nsummary:\n  types:\n  - apiKey\n  notes: >-\n    EPX uses proprietary merchant-credential auth rather than OAuth 2.0. Two\n    documented models exist depending on the integration surface. There is no\n    OAuth authorization server, OIDC discovery, or scope surface, so no\n    scopes/ artifact is produced.\nschemes:\n- name: FourPartKey\n  type: apiKey\n  in: body\n  description: >-\n    Legacy four-part processing key that identifies the merchant on Browser\n    Post API and Hosted Pay Page transaction requests. Composed of four\n    numeric fields sent with each transaction.\n  fields:\n  - CUST_NBR\n  - MERCH_NBR\n  - DBA_NBR\n\
  \  - TERMINAL_NBR\n  used_by:\n  - Browser Post API\n  - Hosted Pay Page\n  - Hosted Checkout\n  source: https://developer.north.com/supplemental-resources/epx-data-dictionary/transaction-request-fields\n- name: EPISignature\n  type: apiKey\n  in: header\n  description: >-\n    HMAC-style request signing for the North EPX Custom Pay REST API. The\n    caller sends an identity header plus a computed signature over the request,\n    provisioned by the North integrations team. Signature computation is\n    documented in the \"How To Authenticate\" section of the Custom Pay API\n    Integration Guide.\n  headers:\n  - EPI-Id\n  - EPI-Signature\n  - EPI-Trace\n  used_by:\n  - North EPX Custom Pay REST API\n  source: https://developer.north.com/blog/tutorial-nodejs-browser-post-custom-pay-api\ntokenization:\n  name: BRIC\n  description: >-\n    Every transaction returns a unique BRIC token that represents the stored\n    payment credential, so cardholder data is never handled by the merchant\
  \ on\n    subsequent operations (e.g. refund/{BRIC}).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/electronic-payment-exchange-inc/refs/heads/main/authentication/electronic-payment-exchange-inc-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Payments
- Payment Processing
- Merchant Acquiring
- Payment Gateway
- Tokenization
- Credit Card Processing
- ACH
- Fintech
---
