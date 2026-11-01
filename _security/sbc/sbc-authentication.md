---
anonymous_access: false
api_key_in: []
api_specs:
- filename: sbc-openapi-generated.yml
  format: yaml
  label: SBC API
  slug: sbc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sbc/openapi/_ae-authored/sbc-openapi-generated.yml
auth_types: []
description: Money-moving Swap API routes are authenticated with a partner API key, sent as an x‑api‑key header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Sbc Authentication
name_suffix: Authentication
oauth_flows: []
overview: SBC declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: SBC
provider_slug: sbc
scheme_count: 1
schemes:
- evidence: Money-moving Swap API routes are authenticated with a partner API key , sent as an x-api-key header.
  header: x-api-key
  how_to_obtain: Create a key yourself at dashboard.stablecoin.xyz after signing in with SIWE.
  location: header
  name: partner API key
  type: apiKey
slug: sbc-authentication
source_filename: sbc-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.stablecoin.xyz/swap/authentication
source_yaml: "generated: '2026-10-26'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.stablecoin.xyz/swap/authentication\nsources:\n- https://docs.stablecoin.xyz/swap/authentication\n- https://docs.stablecoin.xyz/swap/quotes\n- https://docs.stablecoin.xyz/\n- https://docs.stablecoin.xyz/radius/getting-started\ndescription: Money-moving Swap API routes are authenticated with a partner API key, sent as an x‑api‑key header.\nschemes:\n- type: apiKey\n  name: partner API key\n  evidence: Money-moving Swap API routes are authenticated with a partner API key , sent as an x-api-key header.\n  location: header\n  header: x-api-key\n  how_to_obtain: Create a key yourself at dashboard.stablecoin.xyz after signing in with SIWE.\nnote: Read‑only discovery routes do not require authentication.\ndocs: https://docs.stablecoin.xyz/swap/authentication\n"
source_yaml_url: https://artifacts.apis.io/sbc/authentication/sbc-authentication.yml
summary_line: 1 scheme
tags:
- Company
- FinTech
- Payments
- Stablecoin
- API
---
