---
api_key_in: []
api_specs:
- filename: 2c2p-openapi.yml
  format: yaml
  label: 2C2P Payment Token API
  slug: 2c2p-payment-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2c2p/refs/heads/main/openapi/2c2p-openapi.yml
- filename: 2c2p-openapi.yml
  format: yaml
  label: 2C2P Do Payment API
  slug: 2c2p-do-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2c2p/refs/heads/main/openapi/2c2p-openapi.yml
- filename: 2c2p-openapi.yml
  format: yaml
  label: 2C2P Payment Option API
  slug: 2c2p-payment-option-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2c2p/refs/heads/main/openapi/2c2p-openapi.yml
- filename: 2c2p-openapi.yml
  format: yaml
  label: 2C2P Payment Inquiry API
  slug: 2c2p-payment-inquiry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2c2p/refs/heads/main/openapi/2c2p-openapi.yml
- filename: 2c2p-openapi.yml
  format: yaml
  label: 2C2P Payment Maintenance API
  slug: 2c2p-payment-maintenance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2c2p/refs/heads/main/openapi/2c2p-openapi.yml
- filename: 2c2p-openapi.yml
  format: yaml
  label: 2C2P Card Token & Recurring API
  slug: 2c2p-card-token-recurring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2c2p/refs/heads/main/openapi/2c2p-openapi.yml
- filename: 2c2p-openapi.yml
  format: yaml
  label: 2C2P Exchange Rate API
  slug: 2c2p-exchange-rate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2c2p/refs/heads/main/openapi/2c2p-openapi.yml
auth_types:
- jwt
- hmac
description: ''
kind: authentication
layout: security
method: documented
name: 2C2P Authentication
name_suffix: Authentication
oauth_flows: []
overview: 2C2P secures its APIs with jwt and hmac across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: 2C2P
provider_slug: 2c2p
scheme_count: 1
schemes:
- algorithm: HS256
  description: 2C2P Payment Gateway (PGW v4.3) does not use an HTTP Authorization header. Instead, the entire request body is a JSON Web Token (JWS) whose payload carries the transaction fields and whose signature authenticates the merchant. The merchant signs the JWT with its Secret Key using HMAC SHA-256 (HS256); 2C2P returns a JWT signed the same way, which the merchant verifies and decodes. The merchant is identified by the merchantID field inside the signed payload. Credentials (Merchant ID + Secret Key) are issued via the 2C2P merchant profile after commercial onboarding, separately for sandbox and production.
  name: merchantJwt
  notes: Select endpoints (for example the secured exchangeRate variant) additionally support JWT+JWS with asymmetric signing for enhanced security. The Secure Fields / SecurePay flow tokenizes card data in the browser and returns an encryptedCardInfo (securePayToken) that is then submitted inside the signed Do Payment request, keeping raw card data out of the merchant server.
  parameters:
  - description: Merchant identifier included in the signed JWT payload of every request.
    location: payload
    name: merchantID
  - description: Merchant secret key used as the HMAC SHA-256 key to sign/verify the JWT. Never transmitted.
    location: signing-key
    name: secretKey
  scheme: JWS
  sources:
  - https://developer.2c2p.com/docs/api-payment-token
  - https://developer.2c2p.com/docs/api-payment-inquiry
  - https://developer.2c2p.com/docs/using-securefields
  type: jwt
slug: 2c2p-authentication
source_filename: 2c2p-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: documented\nsource: https://developer.2c2p.com/docs\nsummary:\n  types:\n  - jwt\n  - hmac\nschemes:\n- name: merchantJwt\n  type: jwt\n  scheme: JWS\n  algorithm: HS256\n  description: >-\n    2C2P Payment Gateway (PGW v4.3) does not use an HTTP Authorization header.\n    Instead, the entire request body is a JSON Web Token (JWS) whose payload\n    carries the transaction fields and whose signature authenticates the\n    merchant. The merchant signs the JWT with its Secret Key using HMAC SHA-256\n    (HS256); 2C2P returns a JWT signed the same way, which the merchant verifies\n    and decodes. The merchant is identified by the merchantID field inside the\n    signed payload. Credentials (Merchant ID + Secret Key) are issued via the\n    2C2P merchant profile after commercial onboarding, separately for sandbox\n    and production.\n  parameters:\n  - name: merchantID\n    location: payload\n    description: Merchant identifier included in the\
  \ signed JWT payload of every request.\n  - name: secretKey\n    location: signing-key\n    description: Merchant secret key used as the HMAC SHA-256 key to sign/verify the JWT. Never transmitted.\n  notes: >-\n    Select endpoints (for example the secured exchangeRate variant) additionally\n    support JWT+JWS with asymmetric signing for enhanced security. The Secure\n    Fields / SecurePay flow tokenizes card data in the browser and returns an\n    encryptedCardInfo (securePayToken) that is then submitted inside the signed\n    Do Payment request, keeping raw card data out of the merchant server.\n  sources:\n  - https://developer.2c2p.com/docs/api-payment-token\n  - https://developer.2c2p.com/docs/api-payment-inquiry\n  - https://developer.2c2p.com/docs/using-securefields\nsandboxHost: https://sandbox-pgw.2c2p.com\nproductionHost: https://pgw.2c2p.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/2c2p/refs/heads/main/authentication/2c2p-authentication.yml
summary_line: jwt/hmac · 1 scheme
tags:
- Payments
- Payment Gateway
- Southeast Asia
- Singapore
- Thailand
- Cards
- E-Wallet
- Payment Token
- Cross-Border
- Fintech
---
