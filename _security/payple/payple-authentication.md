---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Payple Authentication
name_suffix: Authentication
oauth_flows: []
overview: Payple declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Payple
provider_slug: payple
scheme_count: 3
schemes:
- description: Partner ID (server-side).
  in: body
  name: PCD_CST_ID
  type: apiKey
- description: Partner auth key (server-side).
  in: body
  name: PCD_CUST_KEY
  type: apiKey
- description: Client key (browser payment window).
  in: body
  name: clientKey
  type: apiKey
slug: payple-authentication
source_filename: payple-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://developer.payple.kr/parameters/domestic-card/app\nnotes: >-\n  Payple uses a two-stage credential model rather than OAuth2. There is no\n  OpenAPI-declared securityScheme; this profile is captured from the developer\n  documentation. No OAuth scopes exist, so scopes/ is intentionally omitted.\nmodel: partner-key + client-key\nstages:\n  - stage: client-side\n    name: Client authentication (payment window)\n    mechanism: clientKey\n    where: JavaScript payment-window initialization in the browser\n    parameters:\n      - name: clientKey\n        description: Public client key used to initialize the Payple payment window.\n    restrictions:\n      - Domain / Referer verification (payment window will not open on unregistered domains).\n      - HTTPS required.\n  - stage: server-side\n    name: Partner authentication (approval)\n    mechanism: partner-key -> auth token\n    where: Server-to-server auth request; returns\
  \ a short-lived auth token used for approval.\n    parameters:\n      - name: PCD_CST_ID\n        description: Partner (merchant) identifier issued by Payple.\n      - name: PCD_CUST_KEY\n        description: Partner authentication key issued by Payple.\n    returns:\n      - name: PCD_AUTH_KEY\n        description: Auth key returned from partner authentication, used for the subsequent approval request.\n      - name: PCD_PAY_REQKEY\n        description: Payment request key returned in the result, used for the subsequent approval request.\n    restrictions:\n      - IP allowlist enforced on server-side requests.\n      - Auth token / auth key is short-lived and single-use per approval.\nschemes:\n  - type: apiKey\n    name: PCD_CST_ID\n    in: body\n    description: Partner ID (server-side).\n  - type: apiKey\n    name: PCD_CUST_KEY\n    in: body\n    description: Partner auth key (server-side).\n  - type: apiKey\n    name: clientKey\n    in: body\n    description: Client key (browser\
  \ payment window).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payple/refs/heads/main/authentication/payple-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Payments
- Payment Gateway
- Fintech
- Korea
- Recurring Payments
- Billing
- Cards
- Bank Transfer
---
