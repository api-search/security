---
anonymous_access: false
api_key_in: []
api_specs:
- filename: coil-trade-access-keys-api-openapi.yml
  format: yaml
  label: Coil Access & Keys API
  slug: coil-trade-access-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coil-trade/openapi/coil-trade-access-keys-api-openapi.yml
- filename: coil-trade-change-detection-api-openapi.yml
  format: yaml
  label: Coil Change Detection API
  slug: coil-trade-change-detection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coil-trade/openapi/coil-trade-change-detection-api-openapi.yml
- filename: coil-trade-coil-live-api-openapi.yml
  format: yaml
  label: Coil Coil Live API
  slug: coil-trade-coil-live-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coil-trade/openapi/coil-trade-coil-live-api-openapi.yml
- filename: coil-trade-market-data-api-openapi.yml
  format: yaml
  label: Coil Market Data API
  slug: coil-trade-market-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coil-trade/openapi/coil-trade-market-data-api-openapi.yml
- filename: coil-trade-paid-reads-api-openapi.yml
  format: yaml
  label: Coil Paid reads API
  slug: coil-trade-paid-reads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coil-trade/openapi/coil-trade-paid-reads-api-openapi.yml
- filename: coil-trade-research-api-openapi.yml
  format: yaml
  label: Coil Research API
  slug: coil-trade-research-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coil-trade/openapi/coil-trade-research-api-openapi.yml
- filename: coil-trade-verification-api-openapi.yml
  format: yaml
  label: Coil Verification API
  slug: coil-trade-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coil-trade/openapi/coil-trade-verification-api-openapi.yml
auth_types: []
description: Authentication methods for Coil API as documented on auth.md and quickstart pages.
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Coil Trade Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coil declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Coil
provider_slug: coil-trade
scheme_count: 4
schemes:
- evidence: Free API key | `api_key` | free (email registration) | `X-Coil-Key`
  header: X-Coil-Key
  how_to_obtain: POST https://coil.trade/api/key with an email address; response includes a "key" to use as X-Coil-Key.
  location: header
  name: Free API key
  type: apiKey
- evidence: Wallet sign-in (SIWX) | signed message (no funds move) | free | `SIGN-IN-WITH-X`
  header: SIGN-IN-WITH-X
  how_to_obtain: Obtain a nonce via GET https://coil.trade/api/auth/nonce?address=... then sign the message and send the base64 signature in the SIGN-IN-WITH-X header.
  location: header
  name: Wallet sign‑in (SIWX)
  type: apiKey
- evidence: 'OAuth bearer | `client_credentials` → JWT | included with the license key | `Authorization: Bearer`'
  header: Authorization
  how_to_obtain: POST https://coil.trade/oauth/token with grant_type=client_credentials, client_id=my-agent, client_secret=YOUR-LICENSE-KEY; response includes access_token.
  location: header
  name: OAuth bearer (client_credentials)
  scopes:
  - board:live
  type: http-bearer
- evidence: x402 payment | none (signed payment) | $0.001–$0.25/read, plus a $0.25 one‑hour Live session
  how_to_obtain: When a request returns HTTP 402 with a PAYMENT-REQUIRED header, sign the listed payment option with a wallet holding USDC and resend the request with PAYMENT-SIGNATURE.
  name: x402 payment
  type: other
slug: coil-trade-authentication
source_filename: coil-trade-authentication.yml
source_heading: Authentication Profile
source_url: https://coil.trade/auth.md
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://coil.trade/auth.md\nsources:\n- https://coil.trade/auth.md\n- https://coil.trade/agents/quickstart\ndescription: Authentication methods for Coil API as documented on auth.md and quickstart pages.\nschemes:\n- type: apiKey\n  name: Free API key\n  evidence: Free API key | `api_key` | free (email registration) | `X-Coil-Key`\n  location: header\n  header: X-Coil-Key\n  how_to_obtain: POST https://coil.trade/api/key with an email address; response includes a \"key\" to use as X-Coil-Key.\n- type: apiKey\n  name: Wallet sign‑in (SIWX)\n  evidence: Wallet sign-in (SIWX) | signed message (no funds move) | free | `SIGN-IN-WITH-X`\n  location: header\n  header: SIGN-IN-WITH-X\n  how_to_obtain: Obtain a nonce via GET https://coil.trade/api/auth/nonce?address=... then sign the message and send the base64 signature in the\n    SIGN-IN-WITH-X header.\n- type: http-bearer\n  name: OAuth\
  \ bearer (client_credentials)\n  evidence: 'OAuth bearer | `client_credentials` → JWT | included with the license key | `Authorization: Bearer`'\n  location: header\n  header: Authorization\n  scopes:\n  - board:live\n  how_to_obtain: POST https://coil.trade/oauth/token with grant_type=client_credentials, client_id=my-agent, client_secret=YOUR-LICENSE-KEY; response\n    includes access_token.\n- type: other\n  name: x402 payment\n  evidence: x402 payment | none (signed payment) | $0.001–$0.25/read, plus a $0.25 one‑hour Live session\n  how_to_obtain: When a request returns HTTP 402 with a PAYMENT-REQUIRED header, sign the listed payment option with a wallet holding USDC and\n    resend the request with PAYMENT-SIGNATURE.\nnote: Anonymous access requires no authentication and is not represented as a scheme. 2 extracted row(s) were dropped because their quote was\n  not on the page.\ndocs: https://coil.trade/auth.md\n"
source_yaml_url: https://artifacts.apis.io/coil-trade/authentication/coil-trade-authentication.yml
summary_line: 4 schemes
tags:
- Finance
- Artificial Intelligence
- Stock-Scanner
- Real-Time Data
- Trading
---
