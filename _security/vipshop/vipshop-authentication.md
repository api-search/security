---
api_key_in:
- query
auth_types:
- apiKey
- signature
description: ''
kind: authentication
layout: security
method: searched
name: Vipshop Authentication
name_suffix: Authentication
oauth_flows: []
overview: VIPShop secures its APIs with apiKey and signature across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: VIPShop
provider_slug: vipshop
scheme_count: 2
schemes:
- credential: app_key (public) + secret (private)
  description: Each developer application is issued an APPKEY (app_key) and SECRET after developer authentication. The app_key identifies the caller; the secret is used to compute the per-request signature and is never transmitted.
  in: query
  name: AppKeySecret
  type: apiKey
- description: Every request carries a computed signature (sign) over the request parameters using the app secret. VOP provides a Signature Verification Tool to validate signatures during integration. Vendor authorization binds an app to the vendor accounts whose data it may access.
  name: RequestSignature
  parameter: sign
  type: signature
slug: vipshop-authentication
source_filename: vipshop-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://vop.vip.com/doccenter/viewdoc/65\ndocs: https://vop.vip.com/home#/console/personal\nsummary:\n  types: [apiKey, signature]\n  api_key_in: [query]\n  oauth2_flows: []\n  note: >-\n    No OpenAPI is published, so this profile is captured from the VOP documentation rather\n    than derived from a spec. VOP uses an app-key + secret credential model with per-request\n    signing (a sign parameter), typical of Chinese e-commerce open platforms.\nschemes:\n  - name: AppKeySecret\n    type: apiKey\n    in: query\n    credential: app_key (public) + secret (private)\n    description: >-\n      Each developer application is issued an APPKEY (app_key) and SECRET after developer\n      authentication. The app_key identifies the caller; the secret is used to compute the\n      per-request signature and is never transmitted.\n  - name: RequestSignature\n    type: signature\n    parameter: sign\n    description: >-\n      Every request\
  \ carries a computed signature (sign) over the request parameters using the\n      app secret. VOP provides a Signature Verification Tool to validate signatures during\n      integration. Vendor authorization binds an app to the vendor accounts whose data it may access.\ntools:\n  signature_verification: https://vop.vip.com/doccenter/viewdoc/65\nnotes: >-\n  Exact signature hash algorithm and full system-parameter list are documented in the VOP\n  Development Specifications (login-gated); not fabricated here. This is a signature-auth\n  (not OAuth) provider, so scopes/ is intentionally omitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vipshop/refs/heads/main/authentication/vipshop-authentication.yml
summary_line: apiKey/signature · 2 schemes
tags:
- Company
- Consumer
- E-commerce
- Retail
- Flash Sales
- Open Platform
- China
- Orders
- Inventory
- Logistics
---
