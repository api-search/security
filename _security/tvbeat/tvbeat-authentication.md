---
api_key_in: []
auth_types:
- custom-hmac-signature
description: The TVbeat analytics API authenticates every request with a custom HMAC-SHA256 request-signing scheme modelled closely on AWS Signature Version 4. There is no OAuth 2.0, no OpenID Connect, and no bearer-token or simple API-key header — a signature must be computed per request, so no static credential alone grants access.
kind: authentication
layout: security
method: searched
name: Tvbeat Authentication
name_suffix: Authentication
oauth_flows: []
overview: TVbeat secures its APIs with custom-hmac-signature across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TVbeat
provider_slug: tvbeat
scheme_count: 1
schemes:
- algorithm: HMAC-SHA256
  canonical_request: HTTP_verb + "\n" + canonical_uri + "\n" + canonical_headers + "\n" + signed_headers + "\n" + payload_hash
  canonical_request_notes:
  - canonical_uri excludes protocol, hostname and query string.
  - canonical_headers must include host and x-tvbeat-date, lowercased, trimmed, ASCII-sorted, with a trailing newline.
  - signed_headers is a semicolon-separated list of the header names included (e.g. "host;x-tvbeat-date").
  - payload_hash is the SHA256 hex digest of the request body (SHA256 of the empty string when there is no body).
  constants:
    algorithm: TVBEAT-HMAC-SHA256
    service: ae
  credentials:
  - name: access key ID
    role: public identifier, sent as the Credential component of the Authorization header
  - name: secret
    role: private key material, never transmitted; used to derive the signing key
  headers:
  - name: x-tvbeat-date
    required: true
    value: integer UNIX timestamp of the moment the request was made
  - name: Authorization
    required: true
    value: Algorithm=TVBEAT-HMAC-SHA256, Credential=<access_key>, Service=ae, SignedHeaders=<signed_headers>, Signature=<hex signature>
  key_derivation:
  - key_date = HMAC("TVBEAT" + secret, timestamp)
  - key = HMAC(key_date, service)
  modelled_on: AWS Signature Version 4
  name: TVBEAT-HMAC-SHA256
  provisioning: Both the access key ID and the secret are assigned by TVbeat when an account is opened. There is no self-serve key issuance and no published key-rotation policy.
  replay_protection: The signed x-tvbeat-date timestamp is folded into the key derivation, so a signature is only valid for the timestamp it was generated with. The document does not state a permitted clock-skew window.
  sample_code:
    language: python
    note: The reference publishes a complete Python 2 signing example using hmac/hashlib and requests.
    published: true
  signature: hex(HMAC(derived_key, string_to_sign))
  string_to_sign: algorithm + "\n" + service + "\n" + SHA256(canonical_request)
  type: signature
slug: tvbeat-authentication
source_filename: tvbeat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: >-\n  https://github.com/tvbeat/public/blob/master/docs/api.md#authenticating-your-request\n  — TVbeat's own public API reference, published in the company's GitHub organization\n  (github.com/tvbeat, \"TVbeat public pages\"). No OpenAPI securityScheme exists to\n  derive from; this profile is transcribed from the published prose specification.\ndocs: https://github.com/tvbeat/public/blob/master/docs/api.md\ndescription: >-\n  The TVbeat analytics API authenticates every request with a custom HMAC-SHA256\n  request-signing scheme modelled closely on AWS Signature Version 4. There is no\n  OAuth 2.0, no OpenID Connect, and no bearer-token or simple API-key header — a\n  signature must be computed per request, so no static credential alone grants access.\ncaveat: >-\n  The API root this scheme protects (https://api.tvbeat.com) does not resolve in public\n  DNS as of 2026-08-12 and the reference was last modified 2017-05-23. The\
  \ current\n  TVbeat product documentation at https://docs.tvbeat.com is credential-gated\n  (SnazzyDocs login), so a newer authentication model, if one exists, is not public.\nsummary:\n  types:\n    - custom-hmac-signature\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  static_api_key: false\nschemes:\n  - name: TVBEAT-HMAC-SHA256\n    type: signature\n    algorithm: HMAC-SHA256\n    modelled_on: AWS Signature Version 4\n    credentials:\n      - name: access key ID\n        role: public identifier, sent as the Credential component of the Authorization header\n      - name: secret\n        role: private key material, never transmitted; used to derive the signing key\n    provisioning: >-\n      Both the access key ID and the secret are assigned by TVbeat when an account is\n      opened. There is no self-serve key issuance and no published key-rotation policy.\n    headers:\n      - name: x-tvbeat-date\n        required: true\n        value: integer UNIX timestamp of\
  \ the moment the request was made\n      - name: Authorization\n        required: true\n        value: >-\n          Algorithm=TVBEAT-HMAC-SHA256, Credential=<access_key>, Service=ae,\n          SignedHeaders=<signed_headers>, Signature=<hex signature>\n    canonical_request: >-\n      HTTP_verb + \"\\n\" + canonical_uri + \"\\n\" + canonical_headers + \"\\n\" +\n      signed_headers + \"\\n\" + payload_hash\n    canonical_request_notes:\n      - canonical_uri excludes protocol, hostname and query string.\n      - canonical_headers must include host and x-tvbeat-date, lowercased, trimmed, ASCII-sorted, with a trailing newline.\n      - signed_headers is a semicolon-separated list of the header names included (e.g. \"host;x-tvbeat-date\").\n      - payload_hash is the SHA256 hex digest of the request body (SHA256 of the empty string when there is no body).\n    string_to_sign: algorithm + \"\\n\" + service + \"\\n\" + SHA256(canonical_request)\n    key_derivation:\n      - key_date = HMAC(\"\
  TVBEAT\" + secret, timestamp)\n      - key = HMAC(key_date, service)\n    signature: hex(HMAC(derived_key, string_to_sign))\n    constants:\n      algorithm: TVBEAT-HMAC-SHA256\n      service: ae\n    replay_protection: >-\n      The signed x-tvbeat-date timestamp is folded into the key derivation, so a\n      signature is only valid for the timestamp it was generated with. The document\n      does not state a permitted clock-skew window.\n    sample_code:\n      language: python\n      published: true\n      note: The reference publishes a complete Python 2 signing example using hmac/hashlib and requests.\nauthorization:\n  model: >-\n    Access is scoped per account to one or more named \"datasets\" and to the set of\n    dimensions permitted within them; the dataset name is a path segment\n    (/{dataset}/...). Requesting a dataset or dimension outside the granted\n    permissions returns HTTP 403.\n  scopes_published: false\n  scope_reference: null\nerrors:\n  unauthenticated: 401\
  \ — request was not signed correctly\n  unauthorized: 403 — dataset or dimension outside the caller's access permissions\n  detail: errors/tvbeat-problem-types.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tvbeat/refs/heads/main/authentication/tvbeat-authentication.yml
summary_line: custom-hmac-signature · 1 scheme
tags:
- Company
- Advertising
- AdTech
- Television
- Streaming
- CTV
- Audience Measurement
- Analytics
- Media
---
