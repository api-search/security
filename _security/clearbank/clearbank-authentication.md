---
api_key_in:
- header
api_specs:
- filename: clearbank-accounts-api-openapi.yml
  format: yaml
  label: ClearBank Accounts API
  slug: clearbank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-accounts-api-openapi.yml
- filename: clearbank-cop-api-openapi.yml
  format: yaml
  label: ClearBank Co P API
  slug: clearbank-cop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-cop-api-openapi.yml
- filename: clearbank-createfxquoteendpoint-api-openapi.yml
  format: yaml
  label: ClearBank Create Fx Quote Endpoint API
  slug: clearbank-createfxquoteendpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-createfxquoteendpoint-api-openapi.yml
- filename: clearbank-customer-api-openapi.yml
  format: yaml
  label: ClearBank Customer API
  slug: clearbank-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-customer-api-openapi.yml
- filename: clearbank-customer-due-diligence-api-openapi.yml
  format: yaml
  label: ClearBank Customer Due Diligence API
  slug: clearbank-customer-due-diligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-customer-due-diligence-api-openapi.yml
- filename: clearbank-externalcrossbordercustomerpaymentsv4-api-openapi.yml
  format: yaml
  label: ClearBank External Cross Border Customer Payments V4 API
  slug: clearbank-externalcrossbordercustomerpaymentsv4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-externalcrossbordercustomerpaymentsv4-api-openapi.yml
- filename: clearbank-externalcustomerpaymentsv6-api-openapi.yml
  format: yaml
  label: ClearBank External Customer Payments V6 API
  slug: clearbank-externalcustomerpaymentsv6-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-externalcustomerpaymentsv6-api-openapi.yml
- filename: clearbank-externalinstitutionpaymentsv6-api-openapi.yml
  format: yaml
  label: ClearBank External Institution Payments V6 API
  slug: clearbank-externalinstitutionpaymentsv6-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-externalinstitutionpaymentsv6-api-openapi.yml
- filename: clearbank-externalreturnpaymentsv6-api-openapi.yml
  format: yaml
  label: ClearBank External Return Payments V6 API
  slug: clearbank-externalreturnpaymentsv6-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-externalreturnpaymentsv6-api-openapi.yml
- filename: clearbank-fpspayments-api-openapi.yml
  format: yaml
  label: ClearBank Fps Payments API
  slug: clearbank-fpspayments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-fpspayments-api-openapi.yml
- filename: clearbank-fx-orders-api-openapi.yml
  format: yaml
  label: ClearBank Fx Orders API
  slug: clearbank-fx-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-fx-orders-api-openapi.yml
- filename: clearbank-payments-api-openapi.yml
  format: yaml
  label: ClearBank Payments API
  slug: clearbank-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-payments-api-openapi.yml
- filename: clearbank-retail-api-openapi.yml
  format: yaml
  label: ClearBank Retail API
  slug: clearbank-retail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-retail-api-openapi.yml
- filename: clearbank-sct-payments-api-openapi.yml
  format: yaml
  label: ClearBank SCT Payments API
  slug: clearbank-sct-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-sct-payments-api-openapi.yml
- filename: clearbank-secondaryreferencedata-api-openapi.yml
  format: yaml
  label: ClearBank Secondary Reference Data API
  slug: clearbank-secondaryreferencedata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-secondaryreferencedata-api-openapi.yml
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
