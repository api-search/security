---
api_key_in: []
api_specs:
- filename: postman.yaml
  format: yaml
  label: MoMo All-in-One Payment Gateway (AIO v2)
  slug: aio-payment-gateway
  spec_type: Postman
  url: https://developers.momo.vn/v3/docs/payment/api/other/postman/
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Momo Authentication
name_suffix: Authentication
oauth_flows: []
overview: MoMo declares 7 security scheme(s) across its OpenAPI definitions.
provider_name: MoMo
provider_slug: momo
scheme_count: 7
schemes:
- api: momo:aio-payment-gateway
  docs: https://developers.momo.vn/v3/docs/payment/api/other/signature/
  fields:
    accessKey: Server access key
    partnerCode: Business account's unique identity
    secretKey: Used to create the digital signature (never transmitted)
    signature: HMAC-SHA256 over an alphabetically ordered key1=value1&key2=value2 string
  id: aio-hmac-signature
  location: body
  scheme: HMAC-SHA256
  signed_payload: A canonical string of the request's fields sorted a-z, e.g. accessKey=$accessKey&amount=$amount&description=$description&orderId=$orderId&partnerCode=$partnerCode&requestId=$requestId&transId=$transId for the refund operation. The exact field list differs per operation and is published on each operation's reference page.
  transport: HTTPS POST, Content-Type application/json; charset=UTF-8
  type: signature
- api: momo:aio-payment-gateway
  docs: https://developers.momo.vn/v3/docs/payment/api/other/RSA/
  id: aio-rsa
  purpose: Encrypt sensitive payload fields (card data on the non-hosted ATM flow, tokenisation binding data) with a MoMo-issued public key.
  scheme: RSA
  type: encryption
- api: momo:aio-payment-gateway
  docs: https://developers.momo.vn/v3/docs/payment/api/other/AES/
  id: aio-aes
  purpose: Decrypt the AES-wrapped callbackToken returned by the tokenisation binding and subscription flows.
  scheme: AES
  type: encryption
- api: momo:business-page-openapi
  companion_field: Partner Id
  docs: https://developers.momo.vn/v3/docs/business-page/start/
  id: business-page-api-key
  in: header
  name: X-API-KEY
  scope_model: The X-API-KEY is bound to the permission groups granted to the partner in the MoMo for Business portal — page management and setup, content/posts, messaging, reporting, customer care. A key only reaches the endpoints its granted groups cover.
  scoped: true
  type: apiKey
- additional_required_header:
    X-Request-Id: Unique UUID per request
  api: momo:voucher-distribution
  docs: https://developers.momo.vn/v3/docs/voucher-distribution/integration-documentation/
  flow: client_credentials
  header_note: MoMo's own documentation names the header "Authentication" in the request header table while describing it as a Bearer token in the prose — a genuine ambiguity in the published contract, recorded here as-is rather than resolved.
  id: voucher-oauth-client-credentials
  presented_as: Authorization header, Bearer token
  request_fields:
    clientId: Identifier provided by MoMo
    clientSecret: Secret provided by MoMo
  token_endpoint: POST {environment-domain}/authentication/login
  token_lifetime_human: 24 hours
  token_lifetime_ms: 86400000
  type: oauth2-like
- api: momo:mini-app-open-api
  docs: https://developers.momo.vn/v3/docs/app-center/development-guideline/components-api-sdk/open-api/catalog-functions/
  grant: authorization-code-like
  id: open-platform-jwt
  standard: Described by MoMo as "based on the industry standard OAuth2.0 authorization mechanism"
  steps:
  - The Mini App calls the getUserAuth Mini API to obtain an authCode (a long-lived JWT, 90-day expiry)
  - The partner backend exchanges authCode for an accessToken (a short-lived JWT, 30-minute expiry) at GET /gateway/open/v1/oauth/accessToken
  - The accessToken is presented as Authorization on subsequent Open API calls and must never be returned to the Mini App client
  test_token_endpoint: https://api.mservice.com.vn/openapi/gateway/open/v1/oauth/accessToken
  token_endpoint: https://openapi.momo.vn/gateway/open/v1/oauth/accessToken
  token_lifetimes:
    accessToken: 30 minutes
    authCode: 90 days
  type: oauth2
- api: momo:mini-app-open-api
  companion_header: M-Timestamp
  construction: Base64UrlEncode(SHA256withRSA(data + M-Timestamp + openSecretKey))
  docs: https://developers.momo.vn/v3/docs/app-center/development-guideline/components-api-sdk/open-api/open-api-security/
  header: OP-Signature
  id: open-platform-signature
  key_rotation: Newly generated keys are NOT applied immediately — they take effect automatically after 7 days (168 hours), or right away if the developer explicitly approves them in Mini App Center. A rollback to the previous keys is available. This is a published, dated rotation policy, which is unusual.
  keys:
    openPrivateKey: RSA private key used to sign requests and decrypt responses
    openPublicKey: RSA public key used to verify responses and encrypt the AES symmetric key
    openSecretKey: Unique per Mini App, provided by Open Platform, mixed into the signature
  payload_encryption:
    flag_header: encrypted
    get_parameter: data
    key_header: requestKey
    scheme: AES symmetric key, RSA-wrapped
  scheme: SHA256withRSA
  type: signature
slug: momo-authentication
source_filename: momo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: >-\n  https://developers.momo.vn/v3/docs/payment/api/other/signature/,\n  https://developers.momo.vn/v3/docs/payment/api/other/RSA/,\n  https://developers.momo.vn/v3/docs/payment/api/other/AES/,\n  https://developers.momo.vn/v3/docs/payment/onboarding/integration-process/,\n  https://developers.momo.vn/v3/docs/business-page/start/,\n  https://developers.momo.vn/v3/docs/voucher-distribution/integration-documentation/,\n  https://developers.momo.vn/v3/docs/app-center/development-guideline/components-api-sdk/open-api/api-specifications/\nnote: >-\n  Derived from MoMo's published documentation, not from a securitySchemes block —\n  MoMo publishes no OpenAPI. Each of MoMo's four public APIs uses a DIFFERENT\n  authentication model, which is the single most important fact for an integrator\n  or an agent: credentials, header names and signing algorithms do not carry\n  across them.\ncredential_issuance:\n  portal: https://business.momo.vn/\n\
  \  portal_name: MoMo for Business (M4B)\n  process: >-\n    Register a merchant profile, integrate against the test environment, complete\n    UAT, verify the account, then request production credentials. Production keys\n    are issued after MoMo review, not self-serve.\n  environments_have_separate_keys: true\nschemes:\n- id: aio-hmac-signature\n  api: momo:aio-payment-gateway\n  type: signature\n  scheme: HMAC-SHA256\n  location: body\n  fields:\n    partnerCode: Business account's unique identity\n    accessKey: Server access key\n    secretKey: Used to create the digital signature (never transmitted)\n    signature: HMAC-SHA256 over an alphabetically ordered key1=value1&key2=value2 string\n  signed_payload: >-\n    A canonical string of the request's fields sorted a-z, e.g.\n    accessKey=$accessKey&amount=$amount&description=$description&orderId=$orderId&partnerCode=$partnerCode&requestId=$requestId&transId=$transId\n    for the refund operation. The exact field list differs per\
  \ operation and is\n    published on each operation's reference page.\n  transport: HTTPS POST, Content-Type application/json; charset=UTF-8\n  docs: https://developers.momo.vn/v3/docs/payment/api/other/signature/\n- id: aio-rsa\n  api: momo:aio-payment-gateway\n  type: encryption\n  scheme: RSA\n  purpose: >-\n    Encrypt sensitive payload fields (card data on the non-hosted ATM flow,\n    tokenisation binding data) with a MoMo-issued public key.\n  docs: https://developers.momo.vn/v3/docs/payment/api/other/RSA/\n- id: aio-aes\n  api: momo:aio-payment-gateway\n  type: encryption\n  scheme: AES\n  purpose: >-\n    Decrypt the AES-wrapped callbackToken returned by the tokenisation binding\n    and subscription flows.\n  docs: https://developers.momo.vn/v3/docs/payment/api/other/AES/\n- id: business-page-api-key\n  api: momo:business-page-openapi\n  type: apiKey\n  in: header\n  name: X-API-KEY\n  companion_field: Partner Id\n  scoped: true\n  scope_model: >-\n    The X-API-KEY is bound\
  \ to the permission groups granted to the partner in the\n    MoMo for Business portal — page management and setup, content/posts, messaging,\n    reporting, customer care. A key only reaches the endpoints its granted groups\n    cover.\n  docs: https://developers.momo.vn/v3/docs/business-page/start/\n- id: voucher-oauth-client-credentials\n  api: momo:voucher-distribution\n  type: oauth2-like\n  flow: client_credentials\n  token_endpoint: POST {environment-domain}/authentication/login\n  request_fields:\n    clientId: Identifier provided by MoMo\n    clientSecret: Secret provided by MoMo\n  token_lifetime_ms: 86400000\n  token_lifetime_human: 24 hours\n  presented_as: Authorization header, Bearer token\n  header_note: >-\n    MoMo's own documentation names the header \"Authentication\" in the request\n    header table while describing it as a Bearer token in the prose — a genuine\n    ambiguity in the published contract, recorded here as-is rather than resolved.\n  additional_required_header:\n\
  \    X-Request-Id: Unique UUID per request\n  docs: https://developers.momo.vn/v3/docs/voucher-distribution/integration-documentation/\n- id: open-platform-jwt\n  api: momo:mini-app-open-api\n  type: oauth2\n  standard: 'Described by MoMo as \"based on the industry standard OAuth2.0 authorization mechanism\"'\n  grant: authorization-code-like\n  steps:\n  - The Mini App calls the getUserAuth Mini API to obtain an authCode (a long-lived JWT, 90-day expiry)\n  - The partner backend exchanges authCode for an accessToken (a short-lived JWT, 30-minute expiry) at GET /gateway/open/v1/oauth/accessToken\n  - The accessToken is presented as Authorization on subsequent Open API calls and must never be returned to the Mini App client\n  token_lifetimes:\n    authCode: 90 days\n    accessToken: 30 minutes\n  token_endpoint: https://openapi.momo.vn/gateway/open/v1/oauth/accessToken\n  test_token_endpoint: https://api.mservice.com.vn/openapi/gateway/open/v1/oauth/accessToken\n  docs: https://developers.momo.vn/v3/docs/app-center/development-guideline/components-api-sdk/open-api/catalog-functions/\n\
  - id: open-platform-signature\n  api: momo:mini-app-open-api\n  type: signature\n  scheme: SHA256withRSA\n  header: OP-Signature\n  companion_header: M-Timestamp\n  construction: Base64UrlEncode(SHA256withRSA(data + M-Timestamp + openSecretKey))\n  keys:\n    openSecretKey: Unique per Mini App, provided by Open Platform, mixed into the signature\n    openPrivateKey: RSA private key used to sign requests and decrypt responses\n    openPublicKey: RSA public key used to verify responses and encrypt the AES symmetric key\n  key_rotation: >-\n    Newly generated keys are NOT applied immediately — they take effect\n    automatically after 7 days (168 hours), or right away if the developer\n    explicitly approves them in Mini App Center. A rollback to the previous keys\n    is available. This is a published, dated rotation policy, which is unusual.\n  payload_encryption:\n    scheme: AES symmetric key, RSA-wrapped\n    key_header: requestKey\n    flag_header: encrypted\n    get_parameter: data\n\
  \  docs: https://developers.momo.vn/v3/docs/app-center/development-guideline/components-api-sdk/open-api/open-api-security/\nnetwork_controls:\n  ip_allowlist:\n    note: >-\n      MoMo publishes the source and destination IP addresses for both\n      environments so merchants can firewall them. This is a real, published\n      network control, not inferred.\n    sandbox:\n      incoming: [210.245.113.71]\n      outgoing: [118.69.210.244, 118.68.171.198]\n    production:\n      incoming: [118.69.212.158]\n      outgoing: [118.69.210.244, 116.103.110.134, 14.161.2.38]\n    source: https://developers.momo.vn/v3/docs/payment/onboarding/integration-process/\nnot_published:\n- No OpenAPI securitySchemes block exists — MoMo publishes no machine-readable spec.\n- No OAuth 2.0 discovery document (/.well-known/oauth-authorization-server) on any host.\n- No OpenID Connect discovery document on any host.\n- No mutual TLS requirement is documented.\n- No published scope strings for the Open Platform\
  \ accessToken; access is governed by user consent roles (see scopes/momo-scopes.yml).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/momo/refs/heads/main/authentication/momo-authentication.yml
summary_line: 7 schemes
tags:
- Payments
- Mobile Payments
- FinTech
- Digital Wallet
- Payment Gateway
- QR Payments
- Disbursement
- Buy Now Pay Later
- E-commerce
- Vietnam
---
