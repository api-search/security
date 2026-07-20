---
api_key_in:
- header
auth_types:
- signature
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Ant Group Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ant Group secures its APIs with signature and apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ant Group
provider_slug: ant-group
scheme_count: 1
schemes:
- algorithm: RSA256
  description: Every Antom (Ant Group Global) API request is signed. The signed content is "POST <http-uri>\n<client-id>.<request-time>.<request-body>", signed with the merchant's private RSA key using SHA256withRSA, base64- then URL-encoded. Antom verifies the request with the merchant's uploaded public key; the merchant verifies Antom responses with Antom's public key.
  headers:
  - description: Identifies the merchant/client (e.g. SANDBOX_5X..., production client id).
    name: Client-Id
  - description: Request timestamp in milliseconds.
    name: Request-Time
  - description: algorithm=RSA256, keyVersion=<version>, signature=<url-encoded-signature>
    name: Signature
  key_management: Merchants generate an RSA key pair and upload the public key to the Antom Dashboard; Antom returns its corresponding public key. Key rotation is supported via keyVersion.
  name: DigitalSignature
  type: signature
slug: ant-group-authentication
source_filename: ant-group-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://docs.antom.com/ac/ams/digital_signature\ndocs: https://docs.antom.com/ac/ams/digital_signature\nsummary:\n  types: [signature, apiKey]\n  api_key_in: [header]\n  signing: RSA256 (SHA256withRSA), asymmetric RSA key pair\nschemes:\n  - name: DigitalSignature\n    type: signature\n    algorithm: RSA256\n    description: >-\n      Every Antom (Ant Group Global) API request is signed. The signed content is\n      \"POST <http-uri>\\n<client-id>.<request-time>.<request-body>\", signed with the\n      merchant's private RSA key using SHA256withRSA, base64- then URL-encoded.\n      Antom verifies the request with the merchant's uploaded public key; the merchant\n      verifies Antom responses with Antom's public key.\n    headers:\n      - name: Client-Id\n        description: Identifies the merchant/client (e.g. SANDBOX_5X..., production client id).\n      - name: Request-Time\n        description: Request timestamp in milliseconds.\n\
  \      - name: Signature\n        description: 'algorithm=RSA256, keyVersion=<version>, signature=<url-encoded-signature>'\n    key_management: >-\n      Merchants generate an RSA key pair and upload the public key to the Antom\n      Dashboard; Antom returns its corresponding public key. Key rotation is\n      supported via keyVersion.\ngateways:\n  - https://open-na-global.alipay.com/ams/api/v1/\n  - region-specific variations available via the SDK EndPointConstants\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ant-group/refs/heads/main/authentication/ant-group-authentication.yml
summary_line: signature/apiKey · 1 scheme
tags:
- Company
- Technology
- Payments
- Fintech
- Digital Wallet
- Cross-Border Payments
- Merchant Services
- Alipay
- Antom
---
