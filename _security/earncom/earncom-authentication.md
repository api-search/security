---
api_key_in: []
auth_types:
- http
- custom-signature
description: ''
kind: authentication
layout: security
method: derived
name: Earncom Authentication
name_suffix: Authentication
oauth_flows: []
overview: Earn.com secures its APIs with http and custom-signature across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Earn.com
provider_slug: earncom
scheme_count: 2
schemes:
- description: Primary scheme. The client signs the concatenation of the request URL, an ISO-8601 timestamp, and the JSON request body with the user's bitcoin wallet key, then sends the signature in the Authorization header alongside the timestamp and username. Effectively a bitcoin-keypair-based HTTP message signature.
  format: 21 <iso8601-timestamp> <username> <signature>
  header: Authorization
  in: header
  name: two1-wallet-signature
  signed_material: url + timestamp + body
  sources:
  - two1/server/rest_client.py
  type: custom-signature
- description: HTTP Basic (username/password, base64) used only for the initial login exchange (POST /users/{username}/) before wallet-signature auth takes over.
  name: basic
  scheme: basic
  sources:
  - two1/server/rest_client.py
  type: http
slug: earncom-authentication
source_filename: earncom-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: https://github.com/21dotco/two1-python/blob/master/two1/server/rest_client.py\nstatus: historical\nnotes: >-\n  Earn.com / 21.co published no OpenAPI. This profile is derived from the\n  first-party two1 client library's REST client, which is the only surviving\n  authoritative description of how the api.21.co API was authenticated. The API\n  is no longer reachable (api.21.co is NXDOMAIN as of 2026-07-20).\nsummary:\n  types: [http, custom-signature]\n  api_key_in: []\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\nschemes:\n- name: two1-wallet-signature\n  type: custom-signature\n  in: header\n  header: Authorization\n  format: '21 <iso8601-timestamp> <username> <signature>'\n  description: >-\n    Primary scheme. The client signs the concatenation of the request URL, an\n    ISO-8601 timestamp, and the JSON request body with the user's bitcoin\n    wallet key, then sends the signature in the Authorization header\
  \ alongside\n    the timestamp and username. Effectively a bitcoin-keypair-based HTTP\n    message signature.\n  signed_material: url + timestamp + body\n  sources: [two1/server/rest_client.py]\n- name: basic\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic (username/password, base64) used only for the initial login\n    exchange (POST /users/{username}/) before wallet-signature auth takes over.\n  sources: [two1/server/rest_client.py]\nadditional_headers:\n- name: User-Agent\n  value: 21/<two1-version>\n- name: From\n  value: <wallet-public-key>@<device-id>\n  description: Binds the request to the caller's wallet public key and device UUID.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/earncom/refs/heads/main/authentication/earncom-authentication.yml
summary_line: http/custom-signature · 2 schemes
tags:
- Company
- Cryptocurrency
- Bitcoin
- Payments
- Acquired
- Defunct
- Messaging
---
