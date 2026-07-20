---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Duplo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Duplo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Duplo
provider_slug: duplo
scheme_count: 1
schemes:
- format: Bearer <YOUR_API_KEY>
  header: Authorization
  in: header
  modes:
  - test
  - live
  name: BearerApiKey
  scheme: bearer
  sources:
  - https://docs.tryduplo.com/en/atlas/guides/auth
  type: http
slug: duplo-authentication
source_filename: duplo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.tryduplo.com/en/atlas/guides/auth\ndocs: https://docs.tryduplo.com/en/atlas/api-content/authentication\napi: Atlas Payments API\nsummary:\n  types: [http]\n  http_scheme: bearer\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    Atlas authenticates every request with an API key presented as a Bearer token. A single\n    base host (https://atlas.tryduplo.com) serves both environments; whether a request runs in\n    test or live mode is determined by which key is used. Test and live keys are issued\n    separately in the Atlas dashboard. Additional hardening: optional IP whitelisting and\n    AES-256-GCM request payload encryption with a per-account encryption key.\nschemes:\n  - name: BearerApiKey\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: 'Bearer <YOUR_API_KEY>'\n    modes:\n      - test    # test-mode keys; do not touch live balances or banking networks\n\
  \      - live    # production keys\n    sources: [https://docs.tryduplo.com/en/atlas/guides/auth]\nextras:\n  ip_whitelisting:\n    supported: true\n    docs: https://docs.tryduplo.com/en/atlas/guides/ip\n  payload_encryption:\n    supported: true\n    algorithm: AES-256-GCM\n    docs: https://docs.tryduplo.com/en/atlas/guides/encryption\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/duplo/refs/heads/main/authentication/duplo-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- FinTech
- Payments
- B2B Payments
- Cross-Border Payments
- Expense Management
- Virtual Accounts
- E-Invoicing
- Foreign Exchange
- Africa
- Nigeria
---
