---
anonymous_access: false
api_key_in: []
api_specs:
- filename: trustly-north-america-openapi.yml
  format: yaml
  label: Trustly North America API
  slug: trustly-north-america-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustly/refs/heads/main/openapi/trustly-north-america-openapi.yml
auth_types:
- http
- signature
description: ''
kind: authentication
layout: security
mechanism_count: 5
method: searched
name: Trustly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trustly Group secures its APIs with http and signature across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Trustly Group
provider_slug: trustly
scheme_count: 5
schemes:
- credentials: accessId (username) and accessKey (password), issued per merchant and per environment (sandbox / production)
  docs: https://amer.developers.trustly.com/api-reference/api
  live_probe:
    body: '{"errors":[{"domain":"com.paywithmybank.merchantgateway.v1.exception.AccessControlException","code":375,"message":"Access not authorized"}]}'
    status: 401
    url: https://sandbox.trustly.one/api/v1/countries
  name: HTTPBasic
  scheme: basic
  sources:
  - openapi/trustly-north-america-openapi.yml
  surface: Trustly North America API
  type: http
- algorithm: HMAC-SHA1 (default) or HMAC-SHA512 (beta, prefixed "HmacSHA512:")
  canonicalisation: concatenate the present parameters in the documented fixed order (accessId, merchantId, description, currency, amount, ... transactionId, onlinePPSubtype), HMAC with accessKey, Base64-encode
  docs: https://amer.developers.trustly.com/integrate/api-fundamentals/secure-requests-and-signature-validation/generate-request-signatures
  key: accessKey
  location: requestSignature property of the request payload / establishData object
  name: requestSignature
  required_for: production API requests and SDK operations (POST /establish and the Lightbox establishData)
  surface: Trustly North America API
  type: signature
- direction: inbound (Trustly -> merchant)
  docs: https://amer.developers.trustly.com/integrate/api-fundamentals/secure-requests-and-signature-validation/validate-the-notification-signature
  location: Authorization header (Basic <base64>) on event-notification POSTs; validate before trusting the event
  name: webhookAuthorization
  surface: Trustly North America API
  type: signature
- credentials: Username and Password of the processing account, sent inside every JSON-RPC Data object (test and live accounts have different passwords)
  docs: https://docs.trustly.com/api/api-protocol
  name: JSONRPCCredentials
  scheme: custom
  surface: Trustly Europe API
  type: http
- algorithm: RSA over SHA-1 (default) or SHA-256/384/512 with prefix alg=RS256; / alg=RS384; / alg=RS512;
  canonicalisation: Base64(sign(Method + UUID + serialise(Data))) where serialise concatenates all scalars, hash keys/values and array values sorted ASCIIbetically, null as empty string
  docs: https://docs.trustly.com/api/authentication
  key: merchant-generated 2048-bit RSA key pair (openssl genrsa); public.pem is registered with Trustly's integration team
  name: RSASignature
  reciprocal: Trustly signs every response and every notification with its own private key; merchants verify with the published TEST / LIVE public keys
  surface: Trustly Europe API
  transport: TLS 1.2 or later only; certificates rotate at least yearly without notice, so do not pin
  type: signature
slug: trustly-authentication
source_filename: trustly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: searched\nsource: openapi/trustly-north-america-openapi.yml\ndocs:\n- https://amer.developers.trustly.com/integrate/api-fundamentals/secure-requests-and-signature-validation/generate-request-signatures\n- https://amer.developers.trustly.com/integrate/core-concepts/webhooks-and-events\n- https://docs.trustly.com/api/authentication\n- https://docs.trustly.com/api/security\nsummary:\n  types:\n  - http\n  - signature\n  note: >-\n    Two surfaces, two models. North America REST: HTTP Basic (accessId:accessKey) on every call, plus an HMAC-SHA1 (or\n    HMAC-SHA512, beta) requestSignature computed over an ordered parameter list with the accessKey, and an Authorization\n    header on inbound webhooks. Europe JSON-RPC: every request carries a username/password pair for the processing account\n    and an RSA signature (SHA-1 default; RS256/RS384/RS512 with an alg= prefix) over Method + UUID + serialised Data made\n    with the merchant's private key;\
  \ Trustly signs every response and notification with its own key, whose TEST and LIVE\n    public keys are published on the authentication page. No OAuth scopes exist on either surface — the \"OAuth\" in the NA\n    docs is the bank-side login flow the end user completes inside the Lightbox, not API authorization.\nschemes:\n- name: HTTPBasic\n  type: http\n  scheme: basic\n  surface: Trustly North America API\n  credentials: accessId (username) and accessKey (password), issued per merchant and per environment (sandbox / production)\n  sources:\n  - openapi/trustly-north-america-openapi.yml\n  docs: https://amer.developers.trustly.com/api-reference/api\n  live_probe:\n    url: https://sandbox.trustly.one/api/v1/countries\n    status: 401\n    body: '{\"errors\":[{\"domain\":\"com.paywithmybank.merchantgateway.v1.exception.AccessControlException\",\"code\":375,\"message\":\"Access not authorized\"}]}'\n- name: requestSignature\n  type: signature\n  surface: Trustly North America API\n \
  \ algorithm: HMAC-SHA1 (default) or HMAC-SHA512 (beta, prefixed \"HmacSHA512:\")\n  key: accessKey\n  location: requestSignature property of the request payload / establishData object\n  canonicalisation: concatenate the present parameters in the documented fixed order (accessId, merchantId, description, currency, amount, ... transactionId, onlinePPSubtype), HMAC with accessKey, Base64-encode\n  required_for: production API requests and SDK operations (POST /establish and the Lightbox establishData)\n  docs: https://amer.developers.trustly.com/integrate/api-fundamentals/secure-requests-and-signature-validation/generate-request-signatures\n- name: webhookAuthorization\n  type: signature\n  surface: Trustly North America API\n  direction: inbound (Trustly -> merchant)\n  location: Authorization header (Basic <base64>) on event-notification POSTs; validate before trusting the event\n  docs: https://amer.developers.trustly.com/integrate/api-fundamentals/secure-requests-and-signature-validation/validate-the-notification-signature\n\
  - name: JSONRPCCredentials\n  type: http\n  scheme: custom\n  surface: Trustly Europe API\n  credentials: Username and Password of the processing account, sent inside every JSON-RPC Data object (test and live accounts have different passwords)\n  docs: https://docs.trustly.com/api/api-protocol\n- name: RSASignature\n  type: signature\n  surface: Trustly Europe API\n  algorithm: RSA over SHA-1 (default) or SHA-256/384/512 with prefix alg=RS256; / alg=RS384; / alg=RS512;\n  key: merchant-generated 2048-bit RSA key pair (openssl genrsa); public.pem is registered with Trustly's integration team\n  canonicalisation: Base64(sign(Method + UUID + serialise(Data))) where serialise concatenates all scalars, hash keys/values and array values sorted ASCIIbetically, null as empty string\n  reciprocal: Trustly signs every response and every notification with its own private key; merchants verify with the published TEST / LIVE public keys\n  transport: TLS 1.2 or later only; certificates rotate at least\
  \ yearly without notice, so do not pin\n  docs: https://docs.trustly.com/api/authentication\ntools:\n- name: Signature tester\n  url: https://docs.trustly.com/api/signature-tester\n- name: Notification tool\n  url: https://docs.trustly.com/api/notification-tool\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trustly/refs/heads/main/authentication/trustly-authentication.yml
summary_line: http/signature · 5 schemes
tags:
- Company
- Payments
- Pay by Bank
- Open Banking
- Account-to-Account
- Payouts
- Direct Debit
- Bank Account Verification
- Identity Verification
- Fintech
- Webhook
- MCP
---
