---
anonymous_access: false
api_key_in: []
api_specs:
- filename: genome-host-to-host-api-openapi.yml
  format: yaml
  label: Genome Host-to-Host API
  slug: genome-host-to-host-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genome/refs/heads/main/openapi/genome-host-to-host-api-openapi.yml
- filename: genome-payouts-api-openapi.yml
  format: yaml
  label: Genome Payouts API
  slug: genome-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genome/refs/heads/main/openapi/genome-payouts-api-openapi.yml
auth_types: []
description: Genome does not run one authentication model — it runs four, one per product surface, and none of them is declared in a machine-readable contract. The harvested OpenAPI carries no components.securitySchemes at all, so every scheme below was read out of the documentation prose and, where noted, confirmed against a live unauthenticated request.
kind: authentication
layout: security
mechanism_count: 6
method: searched
name: Genome Authentication
name_suffix: Authentication
oauth_flows: []
overview: Genome declares 7 security scheme(s) across its OpenAPI definitions.
provider_name: Genome
provider_slug: genome
scheme_count: 7
schemes:
- applies_to:
  - Host-to-Host API (https://api.genome.eu/api/pf/host-to-host)
  - Payout API (https://api.genome.eu/api/pf/payout)
  - Query on Demand API (https://api.genome.eu/api/pf/qod)
  - SEPA Payout API (https://api.genome.eu/api/mp/payout)
  - CHECK transaction API (https://api.genome.eu/api/mp/transaction)
  - Verification of Payee API (https://api.genome.eu/api/mp/payee/verification)
  docs: https://developers.genome.eu/merchants/host-to-host-api/
  failure:
    also: 2013 Bad API credentials
    envelope_code: 2001
    envelope_message: Incorrect value in merchant account or pass field
    http_status: 200
    note: 'Authentication failures are NOT signalled with HTTP 401. Probed 2026-09-12: an unauthenticated POST to https://api.genome.eu/api/pf/host-to-host returns HTTP 200 with {"status":"error","code":1004,"message":"Invalid request"} in the body. An agent that reads the HTTP status alone will treat a rejected call as a success.'
  format: merchant_account string(6-32), merchant_password string(6-32)
  id: merchant-credentials
  in: body
  issued_by: Genome integration team, after merchant account approval
  names:
  - merchant_account
  - merchant_password
  type: apiKey
- applies_to:
  - SEPA Payout API
  - Merchant Platform APIs (/api/mp/*)
  docs: https://developers.genome.eu/list-of-response-codes/
  evidence: Probed 2026-09-12 — an unauthenticated POST to https://api.genome.eu/api/mp/payout returned code 2008 before any credential check, which is what establishes that a source-IP allowlist gates this surface.
  failure:
    envelope_code: 2008
    envelope_message: Access from this IP-address is not available
  id: ip-allowlist
  type: network
- access_token_lifetime_minutes: 30
  additional_required_headers:
  - description: The TPP's eIDAS QWAC certificate, PEM body with boundaries and no line breaks. This is the PSD2 RTS-mandated qualified website authentication certificate, carried as a header rather than negotiated at the TLS layer.
    name: Tpp-Qwac-Certificate
  - description: Unique per-call identifier set by the initiating party.
    name: X-Request-ID
  - description: PSU's IP address, required when the request is actively initiated by the PSU.
    name: PSU-IP-Address
  - description: The AIS consent the call is made under (account and transaction reads).
    name: Consent-ID
  applies_to:
  - PSD2 Account Information Services (AIS)
  - PSD2 Payment Initiation Services (PIS)
  - PSD2 Confirmation of Funds (PIIS)
  authorization_endpoint: https://my.genome.eu/oauth2/authorize
  bearer: Authorization Bearer {access_token}
  concurrent_tokens: One active access token per client per user. Acquiring a new token invalidates any other token the client holds for that user.
  discovery_document: none
  discovery_note: No /.well-known/oauth-authorization-server and no /.well-known/openid-configuration on my.genome.eu — both return the SPA shell (see well-known/genome-well-known.yml). A TPP must read the endpoints out of prose.
  docs: https://developers.genome.eu/psd2-api/
  flow: authorization_code
  id: psd2-oauth2
  onboarding: Registered AISP/PISP only; request access at psd2@genome.eu
  refresh_token: optional
  required_parameters:
  - client_id
  - redirect_uri
  - response_type=code
  - state
  scopes_note: The token response carries a scope field, but Genome publishes no scope reference — the example shows a literal "{scope}" placeholder. No scopes/ artifact is emitted because there is nothing published to record.
  scopes_published: false
  strong_customer_authentication:
    factors:
    - Login at my.genome.eu
    - OTP delivered to the account holder's email or phone
    note: The access token carries no permissions until the account owner approves access, per PSD2 SCA.
    required: true
  token_endpoint: https://my.genome.eu/oauth2/token
  token_endpoint_auth_method: client_secret_basic
  token_request_content_type: application/x-www-form-urlencoded
  type: oauth2
- applies_to:
  - Hosted Payment Page session initiation (https://pay.genome.eu)
  - Financial Pixel Web SDK (iframe and popup)
  claims:
    recommended:
    - VALUE_ORDER_ID
    - VALUE_USER_ID
    - VALUE_SUCCESS_URL
    - VALUE_FAILURE_URL
    required:
    - iss (your API key)
    - sub (order or user id)
    - iat
    - exp
    - jti (fresh unique id per token)
    - VALUE_AMOUNT_ISO
    - VALUE_AMOUNT_RAW
  docs: https://developers.genome.eu/merchants/hosted-payment-page/
  format: JWT (JWS, HS256)
  id: hpp-jwt
  legacy: A pre-JWT signature calculation is still documented under the heading "Deprecated - Legacy signature calculation".
  scheme: bearer
  signing_key_derivation: HMAC key = raw SHA-256 digest of the Payment Page API secret. The raw secret is NOT the signing key — tokens signed with it are always rejected. Genome hashes first to guarantee a 32-byte key regardless of secret length.
  type: http
- algorithm: HmacSHA256
  algorithm_header: X-Signature-Algorithm
  applies_to:
  - Incoming payment notification webhooks
  direction: inbound-to-merchant
  docs: https://developers.genome.eu/webhooks/
  header: X-Signature
  id: callback-hmac
  key: per-customer shared secret configured by Genome
  signed_content: the full callback HTTP request body
  type: signature
  version_header: X-Version
- algorithm: SHA-256 over pipe-joined, key-sorted callback fields with the merchant private signature appended
  applies_to:
  - Host-to-Host transaction callbacks
  - SEPA Payout callbacks
  direction: inbound-to-merchant
  docs: https://developers.genome.eu/sepa-payout-api/
  field: checkSum
  id: callback-checksum
  key: private signature issued by the Genome integration team
  type: signature
- applies_to:
  - Hosted Payment Page callbacks (Genome -> merchant)
  docs: https://developers.genome.eu/merchants/hosted-payment-page/
  id: hpp-api-key-header
  in: header
  name: X-API-Key
  type: apiKey
slug: genome-authentication
source_filename: genome-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: searched\nsource: https://developers.genome.eu/merchants/host-to-host-api/ + https://developers.genome.eu/psd2-api/ + https://developers.genome.eu/merchants/hosted-payment-page/ + https://developers.genome.eu/webhooks/\ndocs: https://developers.genome.eu/\nprovider: Genome\nproviderId: genome\ndescription: >-\n  Genome does not run one authentication model — it runs four, one per product surface, and none of\n  them is declared in a machine-readable contract. The harvested OpenAPI carries no\n  components.securitySchemes at all, so every scheme below was read out of the documentation prose\n  and, where noted, confirmed against a live unauthenticated request.\nnote: >-\n  The dominant model on the merchant surface is credentials IN THE REQUEST BODY: merchant_account and\n  merchant_password are ordinary form/JSON fields, not an Authorization header. That has real\n  consequences for an agent — the secret is in the payload on every call, it appears\
  \ in any body log,\n  and there is no header-level scheme for a proxy or gateway to strip. It also means the OpenAPI\n  cannot express the auth model with a securityScheme, which is why the spec has none.\nschemes:\n- id: merchant-credentials\n  type: apiKey\n  in: body\n  names:\n  - merchant_account\n  - merchant_password\n  applies_to:\n  - Host-to-Host API (https://api.genome.eu/api/pf/host-to-host)\n  - Payout API (https://api.genome.eu/api/pf/payout)\n  - Query on Demand API (https://api.genome.eu/api/pf/qod)\n  - SEPA Payout API (https://api.genome.eu/api/mp/payout)\n  - CHECK transaction API (https://api.genome.eu/api/mp/transaction)\n  - Verification of Payee API (https://api.genome.eu/api/mp/payee/verification)\n  format: merchant_account string(6-32), merchant_password string(6-32)\n  issued_by: Genome integration team, after merchant account approval\n  docs: https://developers.genome.eu/merchants/host-to-host-api/\n  failure:\n    envelope_code: 2001\n    envelope_message:\
  \ Incorrect value in merchant account or pass field\n    also: 2013 Bad API credentials\n    http_status: 200\n    note: >-\n      Authentication failures are NOT signalled with HTTP 401. Probed 2026-09-12: an unauthenticated\n      POST to https://api.genome.eu/api/pf/host-to-host returns HTTP 200 with\n      {\"status\":\"error\",\"code\":1004,\"message\":\"Invalid request\"} in the body. An agent that reads the\n      HTTP status alone will treat a rejected call as a success.\n- id: ip-allowlist\n  type: network\n  applies_to:\n  - SEPA Payout API\n  - Merchant Platform APIs (/api/mp/*)\n  docs: https://developers.genome.eu/list-of-response-codes/\n  failure:\n    envelope_code: 2008\n    envelope_message: Access from this IP-address is not available\n  evidence: >-\n    Probed 2026-09-12 — an unauthenticated POST to https://api.genome.eu/api/mp/payout returned\n    code 2008 before any credential check, which is what establishes that a source-IP allowlist\n    gates this surface.\n\
  - id: psd2-oauth2\n  type: oauth2\n  flow: authorization_code\n  applies_to:\n  - PSD2 Account Information Services (AIS)\n  - PSD2 Payment Initiation Services (PIS)\n  - PSD2 Confirmation of Funds (PIIS)\n  authorization_endpoint: https://my.genome.eu/oauth2/authorize\n  token_endpoint: https://my.genome.eu/oauth2/token\n  token_endpoint_auth_method: client_secret_basic\n  token_request_content_type: application/x-www-form-urlencoded\n  bearer: Authorization Bearer {access_token}\n  access_token_lifetime_minutes: 30\n  refresh_token: optional\n  concurrent_tokens: >-\n    One active access token per client per user. Acquiring a new token invalidates any other token\n    the client holds for that user.\n  required_parameters:\n  - client_id\n  - redirect_uri\n  - response_type=code\n  - state\n  scopes_published: false\n  scopes_note: >-\n    The token response carries a scope field, but Genome publishes no scope reference — the example\n    shows a literal \"{scope}\" placeholder. No\
  \ scopes/ artifact is emitted because there is nothing\n    published to record.\n  discovery_document: none\n  discovery_note: >-\n    No /.well-known/oauth-authorization-server and no /.well-known/openid-configuration on\n    my.genome.eu — both return the SPA shell (see well-known/genome-well-known.yml). A TPP must read\n    the endpoints out of prose.\n  strong_customer_authentication:\n    required: true\n    factors:\n    - Login at my.genome.eu\n    - OTP delivered to the account holder's email or phone\n    note: >-\n      The access token carries no permissions until the account owner approves access, per PSD2 SCA.\n  additional_required_headers:\n  - name: Tpp-Qwac-Certificate\n    description: >-\n      The TPP's eIDAS QWAC certificate, PEM body with boundaries and no line breaks. This is the\n      PSD2 RTS-mandated qualified website authentication certificate, carried as a header rather\n      than negotiated at the TLS layer.\n  - name: X-Request-ID\n    description: Unique\
  \ per-call identifier set by the initiating party.\n  - name: PSU-IP-Address\n    description: PSU's IP address, required when the request is actively initiated by the PSU.\n  - name: Consent-ID\n    description: The AIS consent the call is made under (account and transaction reads).\n  onboarding: Registered AISP/PISP only; request access at psd2@genome.eu\n  docs: https://developers.genome.eu/psd2-api/\n- id: hpp-jwt\n  type: http\n  scheme: bearer\n  format: JWT (JWS, HS256)\n  applies_to:\n  - Hosted Payment Page session initiation (https://pay.genome.eu)\n  - Financial Pixel Web SDK (iframe and popup)\n  signing_key_derivation: >-\n    HMAC key = raw SHA-256 digest of the Payment Page API secret. The raw secret is NOT the signing\n    key — tokens signed with it are always rejected. Genome hashes first to guarantee a 32-byte key\n    regardless of secret length.\n  claims:\n    required:\n    - iss (your API key)\n    - sub (order or user id)\n    - iat\n    - exp\n    - jti (fresh\
  \ unique id per token)\n    - VALUE_AMOUNT_ISO\n    - VALUE_AMOUNT_RAW\n    recommended:\n    - VALUE_ORDER_ID\n    - VALUE_USER_ID\n    - VALUE_SUCCESS_URL\n    - VALUE_FAILURE_URL\n  legacy: >-\n    A pre-JWT signature calculation is still documented under the heading \"Deprecated - Legacy\n    signature calculation\".\n  docs: https://developers.genome.eu/merchants/hosted-payment-page/\n- id: callback-hmac\n  type: signature\n  direction: inbound-to-merchant\n  applies_to:\n  - Incoming payment notification webhooks\n  header: X-Signature\n  algorithm: HmacSHA256\n  algorithm_header: X-Signature-Algorithm\n  version_header: X-Version\n  signed_content: the full callback HTTP request body\n  key: per-customer shared secret configured by Genome\n  docs: https://developers.genome.eu/webhooks/\n- id: callback-checksum\n  type: signature\n  direction: inbound-to-merchant\n  applies_to:\n  - Host-to-Host transaction callbacks\n  - SEPA Payout callbacks\n  field: checkSum\n  algorithm: SHA-256\
  \ over pipe-joined, key-sorted callback fields with the merchant private signature appended\n  key: private signature issued by the Genome integration team\n  docs: https://developers.genome.eu/sepa-payout-api/\n- id: hpp-api-key-header\n  type: apiKey\n  in: header\n  name: X-API-Key\n  applies_to:\n  - Hosted Payment Page callbacks (Genome -> merchant)\n  docs: https://developers.genome.eu/merchants/hosted-payment-page/\nsummary:\n  scheme_count: 7\n  declared_in_openapi: 0\n  oauth2_surfaces: 1\n  mutual_tls_or_qwac: 1\n  transport: TLS 1.2 on api.genome.eu, TLS 1.3 on genome.eu (see security/genome-domain-security.yml)\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genome/refs/heads/main/authentication/genome-authentication.yml
summary_line: 7 schemes
tags:
- Finance
- Payments
- Banking
- Open Banking
- PSD2
- SEPA
- Card Processing
- Payouts
- Electronic Money Institution
- Europe
---
