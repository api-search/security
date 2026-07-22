---
api_key_in:
- header
auth_types:
- apiKey
- hmac-signature
description: ''
kind: authentication
layout: security
method: searched
name: Wacai Authentication
name_suffix: Authentication
oauth_flows: []
overview: wacai secures its APIs with apiKey and hmac-signature across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: wacai
provider_slug: wacai
scheme_count: 2
schemes:
- credential_headers:
  - x-wac-app-key
  - x-wac-access-token
  - x-wac-timestamp
  - x-wac-version
  - x-wac-signature
  description: 'Callers authenticate with an appKey/appSecret pair issued by the Wacai open platform. Each request to the gateway (POST https://open.wacai.com/gw/api_entry) is signed: signPlainText = apiName + "|" + apiVersion + "|" + headerString + "|" + bodyMd5, where headerString is the alphabetically-sorted, ampersand-joined set of signed headers (x-wac-timestamp, x-wac-access-token or x-wac-app-key, x-wac-version). Higher SDK versions drop the token and connect the appKey directly to the gateway.

    '
  in: header
  mode: direct-connect
  name: appKeySignature
  type: apiKey
- in: header
  name: tokenService
  note: Older SDK versions obtain an access token via the token service (wacai-token-sdk) before calls.
  type: apiKey
slug: wacai-authentication
source_filename: wacai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://github.com/wacai/wacai-open-sdk/blob/master/doc/api_sign.md\ndocs: https://github.com/wacai/wacai-open-sdk/tree/master/doc\n# No OpenAPI/OAS is published for the Wacai open platform, so this profile is\n# reconstructed from the official SDK protocol docs (doc/api_auth.md, api_sign.md,\n# api_entry.md). The gateway uses appKey/appSecret HMAC request signing, NOT OAuth2.\nsummary:\n  types: [apiKey, hmac-signature]\n  api_key_in: [header]\n  gateway_entry: https://open.wacai.com/gw/api_entry\nschemes:\n  - name: appKeySignature\n    type: apiKey\n    in: header\n    mode: direct-connect\n    credential_headers:\n      - x-wac-app-key        # app key identifying the caller (direct-connect mode)\n      - x-wac-access-token    # access token (token mode; older SDK versions)\n      - x-wac-timestamp       # request timestamp, participates in signature\n      - x-wac-version         # protocol/interface version\n      - x-wac-signature\
  \       # request signature over apiName|apiVersion|headerString|bodyMd5\n    description: >\n      Callers authenticate with an appKey/appSecret pair issued by the Wacai open\n      platform. Each request to the gateway (POST https://open.wacai.com/gw/api_entry)\n      is signed: signPlainText = apiName + \"|\" + apiVersion + \"|\" + headerString + \"|\" + bodyMd5,\n      where headerString is the alphabetically-sorted, ampersand-joined set of signed\n      headers (x-wac-timestamp, x-wac-access-token or x-wac-app-key, x-wac-version).\n      Higher SDK versions drop the token and connect the appKey directly to the gateway.\n  - name: tokenService\n    type: apiKey\n    in: header\n    note: Older SDK versions obtain an access token via the token service (wacai-token-sdk) before calls.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wacai/refs/heads/main/authentication/wacai-authentication.yml
summary_line: apiKey/hmac-signature · 2 schemes
tags:
- Company
- Fintech
- Personal Finance
- Accounting
- Wealth Management
- Open Platform
- API Gateway
- China
---
