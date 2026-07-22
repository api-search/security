---
api_key_in: []
auth_types:
- jwt-bearer
description: ''
kind: authentication
layout: security
method: searched
name: Powertrade Authentication
name_suffix: Authentication
oauth_flows: []
overview: PowerTrade secures its APIs with jwt-bearer across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: PowerTrade
provider_slug: powertrade
scheme_count: 0
schemes: []
slug: powertrade-authentication
source_filename: powertrade-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://support.power.trade/api/authentication.md\ndocs: https://support.power.trade/api/authentication.md\nsummary:\n  types: [jwt-bearer]\n  scheme: ES256 JWT (JWS)\n  applies_to: all private REST, WebSocket position, and FIX endpoints\nscheme:\n  name: PowerTrade API Key JWT\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  algorithm: ES256\n  key_provisioning: >-\n    Create an account at https://app.power.trade and open Account Profile > API Keys\n    (https://app.power.trade/api-keys) to generate an api_key and private_key.\n  token_generation: >-\n    Sign a JWT with the ES256 algorithm using the private_key. Payload includes sub=api_key,\n    iat, exp, and client=\"api\" (a nonce may be added). A web-based builder is available at\n    https://app.power.trade/jwt-builder.\n  example_payload:\n    sub: \"<api_key>\"\n    iat: \"<unix_seconds>\"\n    exp: \"<unix_seconds>\"\n    client: api\n  libraries_referenced:\n\
  \  - {language: python, library: PyJWT, url: https://pyjwt.readthedocs.io/en/stable/}\n  - {language: node, library: jsrsasign, url: https://github.com/kjur/jsrsasign}\nnotes: >-\n  Public REST/WebSocket market-data endpoints require no authentication. Private endpoints reject\n  missing/expired JWTs with 401. An MFA challenge (v2/mfa/*) may be required (401 with challenge,\n  403 when MFA method requirements are not met). API access is gated by an API License Agreement\n  and, per the API overview, is currently disabled by default pending provider approval.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/powertrade/refs/heads/main/authentication/powertrade-authentication.yml
summary_line: jwt-bearer · 0 schemes
tags:
- Company
- Crypto
- Cryptocurrency
- Derivatives
- Options
- Perpetual Futures
- Trading
- Exchange
- Financial Services
- WebSocket
- FIX
- Market Data
---
