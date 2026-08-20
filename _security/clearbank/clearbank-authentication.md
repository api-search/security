---
api_key_in:
- header
api_specs:
- filename: clearbank-sterling-v4.json
  format: json
  label: ClearBank GBP Accounts API
  slug: clearbank-gbp-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-sterling-v4.json
- filename: clearbank-fps-initiate-payment-v3.json
  format: json
  label: ClearBank Faster Payments API
  slug: clearbank-faster-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-fps-initiate-payment-v3.json
- filename: clearbank-chaps-v6.json
  format: json
  label: ClearBank CHAPS API
  slug: clearbank-chaps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-chaps-v6.json
- filename: clearbank-mccy-accounts-v2.json
  format: json
  label: ClearBank Multi-Currency Accounts API
  slug: clearbank-multi-currency-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-mccy-accounts-v2.json
- filename: clearbank-mccy-payments-v1.json
  format: json
  label: ClearBank Multi-Currency Payments API
  slug: clearbank-multi-currency-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-mccy-payments-v1.json
- filename: clearbank-fx-orchestrator-rfq.json
  format: json
  label: ClearBank FX API
  slug: clearbank-fx-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-fx-orchestrator-rfq.json
- filename: clearbank-sepa-ct-v1.json
  format: json
  label: ClearBank SEPA Credit Transfer API
  slug: clearbank-sepa-credit-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-sepa-ct-v1.json
- filename: clearbank-cop-outbound-v1.json
  format: json
  label: ClearBank Confirmation of Payee API
  slug: clearbank-confirmation-of-payee-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-cop-outbound-v1.json
- filename: clearbank-know-your-customer-v1.json
  format: json
  label: ClearBank Customer Due Diligence (KYC) API
  slug: clearbank-customer-due-diligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-know-your-customer-v1.json
- filename: clearbank-cross-border-v4.json
  format: json
  label: ClearBank Cross-Border Sterling Payments API
  slug: clearbank-cross-border-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-cross-border-v4.json
- filename: clearbank-customers_v2_retail.json
  format: json
  label: ClearBank Retail Embedded Banking Customers API
  slug: clearbank-retail-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-customers_v2_retail.json
auth_types:
- http
- custom-signature
description: ''
kind: authentication
layout: security
method: searched
name: Clearbank Authentication
name_suffix: Authentication
oauth_flows: []
overview: ClearBank secures its APIs with http and custom-signature across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ClearBank
provider_slug: clearbank
scheme_count: 3
schemes:
- description: Bearer API token generated in the ClearBank Portal (Institution > Certificates and Tokens > Generate API Token), scoped by an uploaded certificate signing request. A token is shown once at creation and has a maximum validity of one year.
  header: Authorization
  in: header
  name: Authorization
  scheme: bearer
  type: http
- algorithm: RSA
  description: Required on every request that carries a body. A Base64-encoded RSA signature of the SHA-256 hash of the raw request body, using the private key paired with the certificate registered in the Portal.
  hash: SHA-256
  header: DigitalSignature
  in: header
  name: DigitalSignature
  padding: PKCS#1 v1.5
  type: apiKey
- description: Caller-generated unique identifier (max 83 chars) used for idempotency / duplicate detection over a 24-hour window. Missing/invalid returns 400; a detected duplicate returns 409.
  header: X-Request-Id
  in: header
  name: X-Request-Id
  required: true
  type: apiKey
slug: clearbank-authentication
source_filename: clearbank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://clearbank.github.io/uk/docs/api/getting-started/\nnote: >-\n  ClearBank OpenAPI specs do not declare components.securitySchemes; the auth\n  model below is captured from the developer documentation. Every request is\n  authenticated by a bearer API token AND, for any request carrying a payload,\n  an RSA DigitalSignature over the request body. There is no OAuth surface, so\n  no scopes/ artifact is emitted.\nsummary:\n  types: [http, custom-signature]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: Authorization\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  description: >-\n    Bearer API token generated in the ClearBank Portal (Institution >\n    Certificates and Tokens > Generate API Token), scoped by an uploaded\n    certificate signing request. A token is shown once at creation and has a\n    maximum validity of one year.\n- name: DigitalSignature\n  type: apiKey\n  in:\
  \ header\n  header: DigitalSignature\n  description: >-\n    Required on every request that carries a body. A Base64-encoded RSA\n    signature of the SHA-256 hash of the raw request body, using the private\n    key paired with the certificate registered in the Portal.\n  algorithm: RSA\n  hash: SHA-256\n  padding: PKCS#1 v1.5\n- name: X-Request-Id\n  type: apiKey\n  in: header\n  header: X-Request-Id\n  required: true\n  description: >-\n    Caller-generated unique identifier (max 83 chars) used for idempotency /\n    duplicate detection over a 24-hour window. Missing/invalid returns 400;\n    a detected duplicate returns 409.\nwebhook_verification:\n  description: >-\n    Inbound webhooks are signed by ClearBank; consumers verify the signature,\n    then must respond within 5 seconds with HTTP 200 echoing the Nonce and\n    signed with a valid DigitalSignature. Delivery is at-least-once with retries\n    every 15 minutes for up to 24 hours.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/authentication/clearbank-authentication.yml
summary_line: http/custom-signature · 3 schemes
tags:
- Financial-Services
- Banking
- Banking as a Service
- Embedded Banking
- Payments
- Clearing
- Faster Payments
- CHAPS
- Multi-Currency
- Foreign Exchange
- Open Banking
- United Kingdom
- Fintech
---
