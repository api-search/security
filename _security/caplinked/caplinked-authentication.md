---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Caplinked Authentication
name_suffix: Authentication
oauth_flows: []
overview: Caplinked secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Caplinked
provider_slug: caplinked
scheme_count: 1
schemes:
- description: CapLinked API requests are signed with the account's private key using the HMAC-SHA256 algorithm. The signed payload combines the public API key, the user token, and a request expiration timestamp. Requests are transmitted over TLS.
  headers:
  - description: Public API key that identifies the account.
    name: x-api-key
  - description: User token identifying the user resource making the request.
    name: x-api-user-token
  - description: 'Signature in the form: Method=HMAC-SHA256 Signature=[hash].'
    name: x-api-signature
  - description: Unix UTC timestamp after which the signed request expires (example TTL 1800s / 30 min).
    name: x-api-exp-date
  in: header
  name: HmacRequestSigning
  scheme: HMAC-SHA256
  type: apiKey
slug: caplinked-authentication
source_filename: caplinked-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developer.caplinked.com/getting-started\ndocs: https://developer.caplinked.com/getting-started\nsummary:\n  types:\n  - apiKey\n  scheme: hmac-request-signing\n  algorithm: HMAC-SHA256\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: HmacRequestSigning\n  type: apiKey\n  in: header\n  scheme: HMAC-SHA256\n  description: >-\n    CapLinked API requests are signed with the account's private key using the\n    HMAC-SHA256 algorithm. The signed payload combines the public API key, the\n    user token, and a request expiration timestamp. Requests are transmitted over\n    TLS.\n  headers:\n  - name: x-api-key\n    description: Public API key that identifies the account.\n  - name: x-api-user-token\n    description: User token identifying the user resource making the request.\n  - name: x-api-signature\n    description: 'Signature in the form: Method=HMAC-SHA256 Signature=[hash].'\n  - name: x-api-exp-date\n\
  \    description: Unix UTC timestamp after which the signed request expires (example TTL 1800s / 30 min).\nnotes:\n- Private keys must never be committed to source control and can be reset/rolled at any time.\n- Organization-level public and private keys are supported for signing API requests (added 2017-02-17).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caplinked/refs/heads/main/authentication/caplinked-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Virtual Data Room
- Document Security
- File Sharing
- Due Diligence
- Mergers and Acquisitions
- Digital Rights Management
- Compliance
- Data Room
- Security
---
