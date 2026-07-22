---
api_key_in: []
auth_types:
- session-token
- signature-based
description: Keybase API 1.0 uses a custom challenge/response authentication rather than OAuth. Public read endpoints (user/lookup, key/fetch, merkle/root) require no auth. Authenticated calls use a salt+password login handshake to obtain a session token and CSRF token, and identity mutations are signed with the user's private key and posted to the signature endpoints.
kind: authentication
layout: security
method: searched
name: Keybase Authentication
name_suffix: Authentication
oauth_flows: []
overview: Keybase secures its APIs with session-token and signature-based across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Keybase
provider_slug: keybase
scheme_count: 2
schemes:
- description: 'Session token issued by the login flow (getsalt then login: HMAC of the salted password). Carried as a cookie/session token; paired with a csrf_token for state-changing requests.'
  in: cookie
  name: session
  parameter: session
  source: https://keybase.io/docs/api/1.0/call/login
  type: apiKey
- description: Identity and key mutations (sig/post, sig/post_auth, key/add) are signed with the account's private key (PGP or NaCl) over a chained, Merkle-anchored signature, then posted. sig/next_seqno returns the next sequence number for the signature chain.
  name: signature
  scheme: pgp-nacl
  source: https://keybase.io/docs/api/1.0/call/sig/post
  type: signature
slug: keybase-authentication
source_filename: keybase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://keybase.io/docs/api/1.0\ndocs: https://keybase.io/docs/api/1.0\ndescription: >-\n  Keybase API 1.0 uses a custom challenge/response authentication rather than\n  OAuth. Public read endpoints (user/lookup, key/fetch, merkle/root) require no\n  auth. Authenticated calls use a salt+password login handshake to obtain a\n  session token and CSRF token, and identity mutations are signed with the\n  user's private key and posted to the signature endpoints.\nsummary:\n  types: [session-token, signature-based]\n  oauth2: false\n  public_read: true\nschemes:\n- name: session\n  type: apiKey\n  in: cookie\n  parameter: session\n  description: >-\n    Session token issued by the login flow (getsalt then login: HMAC of the\n    salted password). Carried as a cookie/session token; paired with a\n    csrf_token for state-changing requests.\n  source: https://keybase.io/docs/api/1.0/call/login\n- name: signature\n  type: signature\n\
  \  scheme: pgp-nacl\n  description: >-\n    Identity and key mutations (sig/post, sig/post_auth, key/add) are signed\n    with the account's private key (PGP or NaCl) over a chained,\n    Merkle-anchored signature, then posted. sig/next_seqno returns the next\n    sequence number for the signature chain.\n  source: https://keybase.io/docs/api/1.0/call/sig/post\npublic_endpoints:\n- user/lookup\n- key/fetch\n- merkle/root\n- merkle/block\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keybase/refs/heads/main/authentication/keybase-authentication.yml
summary_line: session-token/signature-based · 2 schemes
tags:
- Company
- Security
- Encryption
- Cryptography
- Identity
- Messaging
- Key Management
- PGP
- Developer Tools
---
