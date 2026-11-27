---
anonymous_access: false
api_key_in: []
auth_types: []
description: Neonjelly uses API keys presented as bearer tokens or custom header values.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Neonjelly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Neonjelly declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Neonjelly
provider_slug: neonjelly-io
scheme_count: 1
schemes:
- evidence: 'Clients that can send headers:

    - `Authorization: Bearer nj_…` or `njc_…`'
  header: Authorization
  how_to_obtain: Minted via trial start (`/start` or `POST /v1/trial`) or purchased through Stripe Checkout; the secret (`nj_…`) is shown once at mint.
  location: header
  name: Authorization Bearer
  type: http-bearer
slug: neonjelly-io-authentication
source_filename: neonjelly-io-authentication.yml
source_heading: Authentication Profile
source_url: https://neonjelly.io/docs/auth-and-keys.md
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://neonjelly.io/docs/auth-and-keys.md\nsources:\n- https://neonjelly.io/docs/auth-and-keys.md\n- https://neonjelly.io/docs/auth-and-keys\n- https://neonjelly.io/docs/getting-started.md\n- https://neonjelly.io/docs/getting-started\ndescription: Neonjelly uses API keys presented as bearer tokens or custom header values.\nschemes:\n- type: http-bearer\n  name: Authorization Bearer\n  evidence: 'Clients that can send headers:\n\n    - `Authorization: Bearer nj_…` or `njc_…`'\n  location: header\n  header: Authorization\n  how_to_obtain: Minted via trial start (`/start` or `POST /v1/trial`) or purchased through Stripe Checkout; the secret (`nj_…`) is shown once\n    at mint.\nnote: No OAuth2 flows, http-basic, jwt, hmac, mtls, or other authentication schemes are documented. 1 extracted row(s) were dropped because their\n  quote was not on the page.\ndocs: https://neonjelly.io/docs/auth-and-keys.md\n"
source_yaml_url: https://artifacts.apis.io/neonjelly-io/authentication/neonjelly-io-authentication.yml
summary_line: 1 scheme
tags:
- E-Commerce
- Data
- Artificial Intelligence
- Shopify
- Analytics
---
