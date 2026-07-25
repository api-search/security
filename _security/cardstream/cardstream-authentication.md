---
api_key_in:
- form-body
auth_types:
- merchantID
- password
- message-signing
- ip-allowlist
description: ''
kind: authentication
layout: security
method: searched
name: Cardstream Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cardstream secures its APIs with merchantID, password, message-signing, and ip-allowlist across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cardstream
provider_slug: cardstream
scheme_count: 4
schemes:
- description: Every request must carry the merchantID identifying which Merchant Account the transaction is for. This is the base identity credential.
  field: merchantID
  in: form-body
  name: merchantID
  required: true
  type: apiKey
- description: Optional per-account password. Discouraged for browser-posted forms because the password can appear in client-side code. An incorrect password aborts the transaction with an error response.
  field: merchantPwd
  in: form-body
  name: merchantPwd
  required: false
  type: apiKey
- algorithm: SHA-512
  description: HMAC-style message signing. A signing secret phrase is configured per Merchant Account in the MMS. The client sorts request fields by ascending ASCII field-name order, serialises them (URL-encoded), appends the secret, and hashes with SHA-512; the resulting hash is sent in the signature field. The Gateway re-generates and compares the hash to detect tampering, and returns a signed response plus signed callback POSTs. Signing may be mandatory on some accounts (secret can be changed but not removed).
  field: signature
  in: form-body
  name: signature
  required: conditional
  type: message-signing
- description: Per-account IP allow-lists configured in the MMS, with separate lists for standard requests (e.g. sales) and advanced requests (e.g. refunds, cancellations). Requests from other addresses are aborted.
  name: ip-allowlist
  required: false
  type: network
slug: cardstream-authentication
source_filename: cardstream-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: https://guides.gitbook.io/integrationguide/getting-started/setting-up-your-integration/authentication\ndocs: https://guides.gitbook.io/integrationguide/getting-started/setting-up-your-integration/authentication\nnote: >-\n  Cardstream's Gateway is a form-post API with no OAuth2, OpenID Connect or\n  mTLS/FAPI surface (probes for /.well-known/openid-configuration and\n  /.well-known/oauth-authorization-server return 404). There are no OAuth scopes,\n  so no scopes/ artifact is produced. Auth is a layered model of merchant\n  identification plus optional integrity, credential and network controls\n  configured per Merchant Account in the Merchant Management System (MMS).\nsummary:\n  types: [merchantID, password, message-signing, ip-allowlist]\n  api_key_in: [form-body]\n  transport: HTTP POST application/x-www-form-urlencoded over TLS 1.2+\nschemes:\n  - name: merchantID\n    type: apiKey\n    in: form-body\n    field: merchantID\n\
  \    required: true\n    description: >-\n      Every request must carry the merchantID identifying which Merchant Account\n      the transaction is for. This is the base identity credential.\n  - name: merchantPwd\n    type: apiKey\n    in: form-body\n    field: merchantPwd\n    required: false\n    description: >-\n      Optional per-account password. Discouraged for browser-posted forms because\n      the password can appear in client-side code. An incorrect password aborts\n      the transaction with an error response.\n  - name: signature\n    type: message-signing\n    in: form-body\n    field: signature\n    algorithm: SHA-512\n    required: conditional\n    description: >-\n      HMAC-style message signing. A signing secret phrase is configured per\n      Merchant Account in the MMS. The client sorts request fields by ascending\n      ASCII field-name order, serialises them (URL-encoded), appends the secret,\n      and hashes with SHA-512; the resulting hash is sent in the signature\
  \ field.\n      The Gateway re-generates and compares the hash to detect tampering, and\n      returns a signed response plus signed callback POSTs. Signing may be\n      mandatory on some accounts (secret can be changed but not removed).\n  - name: ip-allowlist\n    type: network\n    required: false\n    description: >-\n      Per-account IP allow-lists configured in the MMS, with separate lists for\n      standard requests (e.g. sales) and advanced requests (e.g. refunds,\n      cancellations). Requests from other addresses are aborted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cardstream/refs/heads/main/authentication/cardstream-authentication.yml
summary_line: merchantID/password/message-signing/ip-allowlist · 4 schemes
tags:
- Payments
- United Kingdom
- Payment Gateway
- Payment Processing
- White Label
- Card Payments
- Acquiring
- Hosted Payment Pages
- Tokenization
- 3-D Secure
- Alternative Payment Methods
- Subscriptions
---
