---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Limepay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Limepay declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Limepay
provider_slug: limepay
scheme_count: 3
schemes:
- applies_to: Limepay Checkout, client-side order/payment initiation
  audience: frontend / Checkout (browser-safe)
  format: Bearer <publishable_api_key>
  header: Authorization
  id: publishable_key
  in: header
  scheme: bearer
  type: http
- applies_to: Payments API (create/pay orders, capture/void, refunds, saved cards)
  audience: server-to-server
  format: Bearer <secret_api_key>
  header: Authorization
  id: secret_key
  in: header
  scheme: bearer
  type: http
- applies_to: Platform API (sub-merchant onboarding, KYC, settlement reports, platform refunds)
  audience: platform administration
  format: Bearer <platform_api_key>
  header: Authorization
  id: platform_key
  in: header
  scheme: bearer
  type: http
slug: limepay-authentication
source_filename: limepay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: derived\nsource: >-\n  Documented Limepay authentication model as captured in apis.yml (developer\n  portal docs.limepay.com.au now gated behind a Redocly login, so no live spec\n  could be re-fetched). No OpenAPI available to run derive-authentication.py\n  against; profile hand-derived from the historically public documentation.\nsummary: >-\n  Limepay used three scoped API keys, each presented as an HTTP Bearer token.\n  A Publishable key authorised frontend/checkout calls, a Secret key authorised\n  server-to-server Payments API calls, and a Platform key authorised\n  administrative marketplace/onboarding calls on the Platform API.\nschemes:\n- id: publishable_key\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Bearer <publishable_api_key>'\n  audience: frontend / Checkout (browser-safe)\n  applies_to: Limepay Checkout, client-side order/payment initiation\n- id: secret_key\n  type: http\n  scheme: bearer\n\
  \  in: header\n  header: Authorization\n  format: 'Bearer <secret_api_key>'\n  audience: server-to-server\n  applies_to: Payments API (create/pay orders, capture/void, refunds, saved cards)\n- id: platform_key\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Bearer <platform_api_key>'\n  audience: platform administration\n  applies_to: Platform API (sub-merchant onboarding, KYC, settlement reports, platform refunds)\noauth2: false\nopenid_connect: false\nmutual_tls: false\nnotes: >-\n  Keys were issued per environment (test vs live). No OAuth2/OIDC flow was\n  documented; authorization is a static bearer API key with resource scope\n  determined by which key is used.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/limepay/refs/heads/main/authentication/limepay-authentication.yml
summary_line: 3 schemes
tags:
- Payments
- Australia
- BNPL
- Payment Gateway
- Checkout
- Embedded Payments
- White Label
- Card Payments
- Marketplace
- Instalments
---
