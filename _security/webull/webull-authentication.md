---
api_key_in:
- header
auth_types:
- apiKey
- http-signature
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Webull Authentication
name_suffix: Authentication
oauth_flows: []
overview: Webull secures its APIs with apiKey, http-signature, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Webull
provider_slug: webull
scheme_count: 3
schemes:
- description: Every request carries an x-app-key identifier plus an HMAC-SHA1 signature over the request computed with the App Secret. The secret is never transmitted.
  headers:
  - name: x-app-key
    purpose: Unique developer identifier
  - name: x-timestamp
    purpose: Request time, ISO 8601 UTC (YYYY-MM-DDThh:mm:ssZ)
  - name: x-signature
    purpose: Cryptographic signature verifying request authenticity
  - name: x-signature-algorithm
    purpose: Algorithm type (e.g. HMAC-SHA1)
  - name: x-signature-version
    purpose: Algorithm version (e.g. 1.0)
  - name: x-signature-nonce
    purpose: Unique random string per request (replay protection)
  - name: x-version
    purpose: Interface version (accepts v2)
  in: header
  name: AppKeyRequestSigning
  sources:
  - docs
  type: apiKey
- description: For 2FA-enabled accounts an x-access-token is required. The SDK initiates token creation automatically; the user completes verification in the Webull mobile app. Tokens are valid ~15 days and auto-refresh.
  headers:
  - name: x-access-token
    purpose: Reusable access token verified through the Webull App
  in: header
  name: TwoFactorAccessToken
  sources:
  - docs
  type: apiKey
- description: The Connect API provides OAuth 2.0 so third parties can obtain authorization to act on a Webull user's account. Sandbox authorization/login redirect via oauth-open-api.sandbox.webull.com / passport.webull.com.
  name: ConnectOAuth2
  sources:
  - docs
  type: oauth2
slug: webull-authentication
source_filename: webull-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.webull.com/apis/docs/authentication/overview\ndocs: https://developer.webull.com/apis/docs/authentication/overview\nsummary:\n  types: [apiKey, http-signature, oauth2]\n  api_key_in: [header]\n  request_signing: HMAC-SHA1\n  notes: >-\n    Webull OpenAPI trading and market-data requests authenticate with an App Key /\n    App Secret pair. The App Secret never leaves the client — it signs each request.\n    The Connect API additionally offers OAuth 2.0 for third-party authorization of\n    Webull user accounts. All requests must use HTTPS.\nschemes:\n  - name: AppKeyRequestSigning\n    type: apiKey\n    in: header\n    description: >-\n      Every request carries an x-app-key identifier plus an HMAC-SHA1 signature over\n      the request computed with the App Secret. The secret is never transmitted.\n    headers:\n      - name: x-app-key\n        purpose: Unique developer identifier\n      - name: x-timestamp\n\
  \        purpose: Request time, ISO 8601 UTC (YYYY-MM-DDThh:mm:ssZ)\n      - name: x-signature\n        purpose: Cryptographic signature verifying request authenticity\n      - name: x-signature-algorithm\n        purpose: Algorithm type (e.g. HMAC-SHA1)\n      - name: x-signature-version\n        purpose: Algorithm version (e.g. 1.0)\n      - name: x-signature-nonce\n        purpose: Unique random string per request (replay protection)\n      - name: x-version\n        purpose: Interface version (accepts v2)\n    sources: [docs]\n  - name: TwoFactorAccessToken\n    type: apiKey\n    in: header\n    description: >-\n      For 2FA-enabled accounts an x-access-token is required. The SDK initiates token\n      creation automatically; the user completes verification in the Webull mobile app.\n      Tokens are valid ~15 days and auto-refresh.\n    headers:\n      - name: x-access-token\n        purpose: Reusable access token verified through the Webull App\n    sources: [docs]\n  - name: ConnectOAuth2\n\
  \    type: oauth2\n    description: >-\n      The Connect API provides OAuth 2.0 so third parties can obtain authorization to\n      act on a Webull user's account. Sandbox authorization/login redirect via\n      oauth-open-api.sandbox.webull.com / passport.webull.com.\n    sources: [docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/webull/refs/heads/main/authentication/webull-authentication.yml
summary_line: apiKey/http-signature/oauth2 · 3 schemes
tags:
- Company
- Technology
- Financial Services
- Brokerage
- Trading
- Stock Market
- Market Data
- Investing
- Fintech
- Cryptocurrency
---
