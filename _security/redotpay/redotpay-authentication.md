---
api_key_in: []
auth_types: []
description: RedotPay authenticates clients with the OAuth2 Device Authorization Grant (RFC 8628), then makes Bearer-token HTTP requests to the production API. Derived from the first-party redotpay CLI source; no public OpenAPI or hosted auth docs page is published.
kind: authentication
layout: security
method: searched
name: Redotpay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Redotpay declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Redotpay
provider_slug: redotpay
scheme_count: 2
schemes:
- authorization_base: https://app.rp-2023app.com
  client_id: redotpay
  device_authorization_endpoint: /api/v1/oauth/device_authorization
  flow: device_authorization
  grant_type: urn:ietf:params:oauth:grant-type:device_code
  notes: 'Device flow: client requests device_authorization, user approves in the RedotPay App (QR / user_code), client polls the token endpoint. Optional merchant id (`mid`) may be sent on device_authorization. Tokens are stored in the OS credential store by default.'
  scopes:
  - mpp_charge
  token_endpoint: /api/v1/oauth/token
  type: oauth2
- description: 'After device login, API requests carry `Authorization: Bearer <access_token>`. The agentic MPP pay endpoint additionally accepts an `Authorization: Payment` credential returned by the pay flow.'
  scheme: bearer
  type: http
slug: redotpay-authentication
source_filename: redotpay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://github.com/redotpay/redotpay-cli (src/auth.rs, config.example.toml, src/config.rs)\ndescription: >-\n  RedotPay authenticates clients with the OAuth2 Device Authorization Grant (RFC 8628), then makes\n  Bearer-token HTTP requests to the production API. Derived from the first-party redotpay CLI source;\n  no public OpenAPI or hosted auth docs page is published.\nschemes:\n- type: oauth2\n  flow: device_authorization\n  grant_type: urn:ietf:params:oauth:grant-type:device_code\n  authorization_base: https://app.rp-2023app.com\n  device_authorization_endpoint: /api/v1/oauth/device_authorization\n  token_endpoint: /api/v1/oauth/token\n  client_id: redotpay\n  scopes:\n  - mpp_charge\n  notes: >-\n    Device flow: client requests device_authorization, user approves in the RedotPay App (QR / user_code),\n    client polls the token endpoint. Optional merchant id (`mid`) may be sent on device_authorization.\n    Tokens are stored\
  \ in the OS credential store by default.\n- type: http\n  scheme: bearer\n  description: >-\n    After device login, API requests carry `Authorization: Bearer <access_token>`. The agentic MPP pay\n    endpoint additionally accepts an `Authorization: Payment` credential returned by the pay flow.\ntoken_storage: OS credential store (Keychain / Windows Credential Manager / Linux Secret Service); file fallback via REDOTPAY_CLI_OAUTH_STORE=file\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/redotpay/refs/heads/main/authentication/redotpay-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Payments
- Fintech
- Stablecoin
- Cryptocurrency
- Wallet
- Agentic Payments
- Machine Payments Protocol
- x402
- OAuth
---
