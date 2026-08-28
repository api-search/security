---
api_key_in:
- header
api_specs:
- filename: satispay-gbusiness-api.json
  format: json
  label: Satispay GBusiness API
  slug: satispay-gbusiness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/satispay/refs/heads/main/openapi/satispay-gbusiness-api.json
- filename: satispay-production.json
  format: json
  label: Satispay GBusiness API (production surface)
  slug: satispay-gbusiness-production
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/satispay/refs/heads/main/openapi/satispay-production.json
- filename: satispay-sandbox.json
  format: json
  label: Satispay GBusiness API (sandbox)
  slug: satispay-gbusiness-sandbox
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/satispay/refs/heads/main/openapi/satispay-sandbox.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Satispay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Satispay secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Satispay
provider_slug: satispay
scheme_count: 1
schemes:
- detail: 'Authorization: Signature keyId="<KeyId>", algorithm="rsa-sha256", headers="(request-target) host date digest", signature="<base64 RSA-SHA256 signature>"'
  in: header
  name: sec0
  parameter: Authorization
  sources:
  - openapi/satispay-sandbox.json
  type: apiKey
slug: satispay-authentication
source_filename: satispay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: >-\n  https://developers.satispay.com/reference/introduction,\n  https://developers.satispay.com/reference/generate-rsa-keys,\n  https://developers.satispay.com/reference/keyid,\n  https://developers.satispay.com/reference/compose-the-authentication-header,\n  https://developers.satispay.com/reference/testinput, openapi/satispay-sandbox.json\nsummary:\n  model: http-message-signatures\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2: false\n  openid_connect: false\n  mtls: false\n  note: >-\n    Satispay does not use OAuth. Every request to the GBusiness API is signed with an RSA private key\n    following the Signing HTTP Messages (Cavage) draft-10, and the signature travels in the standard\n    Authorization header. The OpenAPI declares this as a generic apiKey-in-header scheme (sec0), which\n    understates the real model — the header value is a computed signature, not a static key.\nschemes:\n- name: sec0\n  type:\
  \ apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/satispay-sandbox.json\n  detail: >-\n    Authorization: Signature keyId=\"<KeyId>\", algorithm=\"rsa-sha256\",\n    headers=\"(request-target) host date digest\", signature=\"<base64 RSA-SHA256 signature>\"\nflow:\n  standard: https://tools.ietf.org/html/draft-cavage-http-signatures-10\n  standard_name: Signing HTTP Messages (Cavage/Sporny draft-10)\n  one_time_setup:\n  - step: 1\n    name: Generate an RSA key pair\n    docs: https://developers.satispay.com/reference/generate-rsa-keys\n  - step: 2\n    name: Exchange the activation code for a KeyId\n    docs: https://developers.satispay.com/reference/keyid\n    operation: keyid\n    endpoint: POST /g_business/v1/authentication_keys\n    request:\n      public_key: RSA public key in PEM format\n      token: the one-time activation code generated in the Satispay Business Dashboard\n    response:\n      key_id: opaque identifier used as the signature keyId for every\
  \ later request\n    note: Activation codes are single use; re-pairing an already-paired token returns error code 45.\n  per_request:\n  - step: 3\n    name: Create the Digest of the body\n    docs: https://developers.satispay.com/reference/create-the-digest\n    header: 'Digest: SHA-256=<base64 sha256 of the raw body>'\n  - step: 4\n    name: Compose the Message (signing string)\n    docs: https://developers.satispay.com/reference/create-the-string\n    components:\n    - (request-target)\n    - host\n    - date\n    - digest\n  - step: 5\n    name: Sign the Message with the RSA private key\n    docs: https://developers.satispay.com/reference/sign-the-string\n    algorithm: rsa-sha256\n  - step: 6\n    name: Compose the Authorization header\n    docs: https://developers.satispay.com/reference/compose-the-authentication-header\nverification:\n  test_endpoint: POST https://staging.authservices.satispay.com/wally-services/protocol/tests/signature\n  operation: testinput\n  docs: https://developers.satispay.com/reference/testinput\n\
  \  note: The test endpoint accepts GET, POST, PUT, DELETE and PATCH and echoes whether the signature verified.\ncredentials:\n  sandbox:\n    obtain: https://satispay-sandbox.paperform.co/\n    docs: https://developers.satispay.com/docs/credentials\n    note: A form request; Satispay emails the staging app links and the staging activation code.\n  production:\n    obtain: https://dashboard.satispay.com\n    docs: https://developers.satispay.com/docs/credentials\n    note: >-\n      Create a Satispay Business account, get the business profile verified, create a shop, then generate\n      the shop's activation code in the Dashboard and exchange it for a KeyId.\ncallback_authentication:\n  docs: https://developers.satispay.com/reference/callback-s2s\n  digest: Every callback carries a Digest header with the SHA-256 of the body.\n  signature: >-\n    Callbacks MAY carry an Authorization header with an asymmetric signature over Digest and Date,\n    verifiable with Satispay's public key. Whether\
  \ a given callback is signed depends on how the\n    integration is configured — Satispay's own docs say not all callbacks are signed.\ndevice_headers:\n  note: >-\n    The KeyId exchange accepts optional x-satispay-* device identification headers that are not\n    authentication but are recorded here because they travel with the credential exchange.\n  headers:\n  - x-satispay-deviceinfo\n  - x-satispay-devicetype\n  - x-satispay-os\n  - x-satispay-osv\n  - x-satispay-apph\n  - x-satispay-appn\n  - x-satispay-appv\n  - x-satispay-tracking-code\n  devicetype_enum:\n  - SMARTPHONE\n  - TABLET\n  - CASH REGISTER\n  - POS\n  - PC\n  - ECOMMERCE_PLUGIN\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/satispay/refs/heads/main/authentication/satispay-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Payments
- Mobile Payments
- Fintech
- E-Money
- E-Commerce
- Italy
- Europe
- Merchant Services
- Recurring Payments
- Refunds
- Meal Vouchers
- Company
---
