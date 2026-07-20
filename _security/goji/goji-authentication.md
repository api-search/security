---
api_key_in: []
auth_types:
- http
- hmac
description: Goji Platform API authentication. Production requests are cryptographically signed using an HMAC-SHA256 mechanism; a Basic HTTP API key and password is available for easier prototyping against the sandbox environment. There is no OAuth 2.0 / OpenID Connect surface -- no scopes artifact applies.
kind: authentication
layout: security
method: searched
name: Goji Authentication
name_suffix: Authentication
oauth_flows: []
overview: Goji secures its APIs with http and hmac across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Goji
provider_slug: goji
scheme_count: 2
schemes:
- description: Each HTTP request is cryptographically signed with a secret private key known only to the API client and Goji. The canonical string is encrypted with HMAC-SHA256 using the private key, the result is Base64 encoded, then UTF-8 URL encoded, and sent in the Authorization header.
  headers:
  - description: The Base64-encoded, URL-encoded HMAC-SHA256 signature of the request.
    name: Authorization
  - description: A unique string for every request; included in the signature string to prevent replay attacks.
    name: x-nonce
  - description: Milliseconds since epoch; included in the signature string to prevent replay attacks.
    name: x-timestamp
  name: hmac
  scheme: hmac-sha256
  sources:
  - docs.api.goji.investments
  type: http
- description: A Basic HTTP API key and password available for easier prototyping against the sandbox environment (api-sandbox.goji.investments). Not for production.
  name: basicAuth
  scheme: basic
  sources:
  - docs.api.goji.investments
  type: http
slug: goji-authentication
source_filename: goji-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.api.goji.investments/\ndocs: https://docs.api.goji.investments/\ndescription: >-\n  Goji Platform API authentication. Production requests are cryptographically\n  signed using an HMAC-SHA256 mechanism; a Basic HTTP API key and password is\n  available for easier prototyping against the sandbox environment. There is no\n  OAuth 2.0 / OpenID Connect surface -- no scopes artifact applies.\nsummary:\n  types: [http, hmac]\n  production: hmac-sha256-signed\n  sandbox: http-basic\nschemes:\n- name: hmac\n  type: http\n  scheme: hmac-sha256\n  description: >-\n    Each HTTP request is cryptographically signed with a secret private key\n    known only to the API client and Goji. The canonical string is encrypted\n    with HMAC-SHA256 using the private key, the result is Base64 encoded, then\n    UTF-8 URL encoded, and sent in the Authorization header.\n  headers:\n  - name: Authorization\n    description: The Base64-encoded,\
  \ URL-encoded HMAC-SHA256 signature of the request.\n  - name: x-nonce\n    description: A unique string for every request; included in the signature string to prevent replay attacks.\n  - name: x-timestamp\n    description: Milliseconds since epoch; included in the signature string to prevent replay attacks.\n  sources: [docs.api.goji.investments]\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: >-\n    A Basic HTTP API key and password available for easier prototyping against\n    the sandbox environment (api-sandbox.goji.investments). Not for production.\n  sources: [docs.api.goji.investments]\nnotes: >-\n  Production API calls must be cryptographically signed. The onboarding flow\n  begins by fetching hosted Terms and Conditions (GET /platformApi/terms) and\n  creating an investor (POST /platformApi/investors), which returns a clientId\n  used on all subsequent calls.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goji/refs/heads/main/authentication/goji-authentication.yml
summary_line: http/hmac · 2 schemes
tags:
- Company
- Fintech
- Private Markets
- Investments
- Funds
- KYC
- Payments
- ISA
- Settlement
- Webhooks
- Euroclear
---
