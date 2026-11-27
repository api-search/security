---
anonymous_access: false
api_key_in: []
auth_types: []
description: NanoParse authenticates requests using a wallet address and an EIP‑191 signature passed in custom HTTP headers for the free tier, and by attaching an x402 v2 payment envelope in the request meta for paid parses.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: NanoParse Authentication
name_suffix: Authentication
oauth_flows: []
overview: NanoParse declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: NanoParse
provider_slug: nanoparse
scheme_count: 2
schemes:
- evidence: 'send the address and the signature with the next call (REST): curl -sS https://nanoparse.app/fetch -H ''Content-Type: application/json'' -H "X-Nanoparse-Wallet: 0xYourAddress" -H "X-Nanoparse-Signature: 0x<65-byte r||s||v>" -d ''{"url":"https://example.com"}'''
  header: X-Nanoparse-Wallet
  how_to_obtain: Sign the exact free‑tier claim string with any Ethereum wallet (EIP‑191 personal_sign) and include the wallet address and signature in the request headers.
  location: header
  name: wallet signature
  type: other
- evidence: Retry nanoparse_fetch with the signed envelope at params._meta["x402/payment"] (x402 v2 MCP transport)
  how_to_obtain: When a payment challenge is returned, build a PaymentPayload envelope signed with EIP‑712 using the wallet, then attach it to the request meta field "x402/payment".
  location: body
  name: x402 payment envelope
  type: other
slug: nanoparse-authentication
source_filename: nanoparse-authentication.yml
source_heading: Authentication Profile
source_url: https://nanoparse.app/quickstart
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://nanoparse.app/quickstart\nsources:\n- https://nanoparse.app/quickstart\ndescription: NanoParse authenticates requests using a wallet address and an EIP‑191 signature passed in custom HTTP headers for the free tier,\n  and by attaching an x402 v2 payment envelope in the request meta for paid parses.\nschemes:\n- type: other\n  name: wallet signature\n  evidence: 'send the address and the signature with the next call (REST): curl -sS https://nanoparse.app/fetch -H ''Content-Type: application/json''\n    -H \"X-Nanoparse-Wallet: 0xYourAddress\" -H \"X-Nanoparse-Signature: 0x<65-byte r||s||v>\" -d ''{\"url\":\"https://example.com\"}'''\n  location: header\n  header: X-Nanoparse-Wallet\n  how_to_obtain: Sign the exact free‑tier claim string with any Ethereum wallet (EIP‑191 personal_sign) and include the wallet address and signature\n    in the request headers.\n- type: other\n\
  \  name: x402 payment envelope\n  evidence: Retry nanoparse_fetch with the signed envelope at params._meta[\"x402/payment\"] (x402 v2 MCP transport)\n  location: body\n  how_to_obtain: When a payment challenge is returned, build a PaymentPayload envelope signed with EIP‑712 using the wallet, then attach it to\n    the request meta field \"x402/payment\".\nnote: No standard apiKey, oauth2, http-bearer, http-basic, jwt, hmac, or mtls schemes are documented.\ndocs: https://nanoparse.app/quickstart\n"
source_yaml_url: https://artifacts.apis.io/nanoparse/authentication/nanoparse-authentication.yml
summary_line: 2 schemes
tags:
- Web Parsing
- AI Agents
- Markdown Conversion
- Litmus Scoring
- Crypto Payments
---
