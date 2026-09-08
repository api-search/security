---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Addx Authentication
name_suffix: Authentication
oauth_flows: []
overview: ADDX declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ADDX
provider_slug: addx
scheme_count: 1
schemes:
- algorithm: HMAC-SHA256
  applies_to: all documented operations
  description: Request signature. The documentation's own Postman sample builds the signed string as [timestamp, method].join("") and computes CryptoJS.HmacSHA256(signature, secret_key).toString(CryptoJS.enc.Base64).
  encoding: base64
  headers:
  - name: X-Signature
    required: true
    value: Signature generated using open-SSL HMAC
  - name: X-UserId
    required: true
    value: Key ID of the user
  - name: X-TimeStamp
    required: true
    value: UTC epoch timestamp in seconds
  id: addx-hmac-signature
  in: header
  scheme: signature
  type: http
slug: addx-authentication
source_filename: addx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: searched\nsource: https://api-docs.addx.co/open-api/\nname: ADDX Open API authentication\napi: ADDX Open API\ndocs: https://api-docs.addx.co/open-api/\nsummary: >-\n  ADDX does not use OAuth, OpenID Connect or a plain bearer API key. Every request to the ADDX Open API is\n  signed: the caller holds a Key ID and a secret passphrase generated from the API-Settings panel in their\n  ADDX user profile, and sends an HMAC-SHA256 signature over the concatenation of a UTC epoch timestamp and\n  the HTTP method, Base64 encoded. The provider states that a user may need more than one key/secret pair\n  depending on which requests they make.\nschemes:\n- id: addx-hmac-signature\n  type: http\n  scheme: signature\n  in: header\n  algorithm: HMAC-SHA256\n  encoding: base64\n  description: >-\n    Request signature. The documentation's own Postman sample builds the signed string as\n    [timestamp, method].join(\"\") and computes CryptoJS.HmacSHA256(signature,\
  \ secret_key).toString(CryptoJS.enc.Base64).\n  headers:\n  - name: X-Signature\n    value: Signature generated using open-SSL HMAC\n    required: true\n  - name: X-UserId\n    value: Key ID of the user\n    required: true\n  - name: X-TimeStamp\n    value: UTC epoch timestamp in seconds\n    required: true\n  applies_to: all documented operations\ncredentials:\n  issuance: self-service, inside the authenticated product\n  where: API-Settings in the User Profile section of the ADDX platform\n  kinds:\n  - Key ID (public identifier, sent as X-UserId)\n  - secret passphrase (never transmitted; used as the HMAC key)\n  multiple_keys: >-\n    The docs state that for security reasons a user may have to generate more than one key/secret pair\n    depending on the API request.\n  rotation_policy_published: false\n  expiry_published: false\noauth2: false\nopenid_connect: false\nmutual_tls: false\napi_key_header: false\nauthorization:\n  model: account-scoped\n  note: >-\n    \"Most resources are\
  \ bound to a specific account belonging to the authenticated user. As the user can\n    control which accounts are accessible accounts, you should make sure you have the access to right\n    account. Otherwise a 404 will be returned.\" A 404 is therefore an authorization signal on this API, not\n    only a routing one.\n  scopes_published: false\n  scope_surface: none — no OAuth scopes or named permissions are documented\ngaps:\n- No published token lifetime, replay window, or clock-skew tolerance for X-TimeStamp.\n- The docs do not state whether the signed string includes the request path or body, only timestamp + method.\n- No key rotation or revocation procedure is documented.\n- No sandbox or test credentials are published; environments are issued per use case on request.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/addx/refs/heads/main/authentication/addx-authentication.yml
summary_line: 1 scheme
tags:
- Digital Securities Exchange
- Private Markets
- Tokenization
- Alternative Investments
- Wealth Management
- Capital Markets
- Fintech
- Digital Assets
- Investment Platform
- Singapore
---
