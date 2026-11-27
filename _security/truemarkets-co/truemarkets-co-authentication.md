---
anonymous_access: false
api_key_in: []
api_specs:
- filename: truemarkets-co-openapi-generated.yml
  format: yaml
  label: True Markets API
  slug: truemarkets-co-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/truemarkets-co/openapi/_ae-authored/truemarkets-co-openapi-generated.yml
auth_types: []
description: Authentication schemes for True Markets APIs
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: True Markets Authentication
name_suffix: Authentication
oauth_flows: []
overview: True Markets declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: True Markets
provider_slug: truemarkets-co
scheme_count: 2
schemes:
- evidence: 'The response has an access token, which you send in `Authorization: Bearer` on every call.'
  header: Authorization
  how_to_obtain: Sign the `{key_id}.{timestamp}` challenge with your private key (ES256) and POST to `/v1/auth/api-key/token` to receive a JWT access token (and optionally a refresh token).
  location: header
  name: Bearer
  type: http-bearer
- authorize_url: https://api.truemarkets.co/v1/auth/oauth/authorize
  evidence: PKCE is required and `code_challenge_method` must be `S256`.
  how_to_obtain: Use the authorization endpoint with PKCE as described; token endpoint is not documented.
  name: OAuth2
  type: oauth2
slug: truemarkets-co-authentication
source_filename: truemarkets-co-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.truemarkets.co/trading-api/api-key.md
source_yaml: "generated: '2026-11-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.truemarkets.co/trading-api/api-key.md\nsources:\n- https://docs.truemarkets.co/trading-api/api-key.md\n- https://docs.truemarkets.co/openapi/auth.yaml\n- https://docs.truemarkets.co/developer-resources/api-keys.md\n- https://docs.truemarkets.co/developer-resources/authentication.md\ndescription: Authentication schemes for True Markets APIs\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'The response has an access token, which you send in `Authorization: Bearer` on every call.'\n  location: header\n  header: Authorization\n  how_to_obtain: Sign the `{key_id}.{timestamp}` challenge with your private key (ES256) and POST to `/v1/auth/api-key/token` to receive a JWT\n    access token (and optionally a refresh token).\n- type: oauth2\n  name: OAuth2\n  evidence: PKCE is required and `code_challenge_method` must be `S256`.\n  authorize_url: https://api.truemarkets.co/v1/auth/oauth/authorize\n\
  \  how_to_obtain: Use the authorization endpoint with PKCE as described; token endpoint is not documented.\ndocs: https://docs.truemarkets.co/trading-api/api-key.md\n"
source_yaml_url: https://artifacts.apis.io/truemarkets-co/authentication/truemarkets-co-authentication.yml
summary_line: 2 schemes
tags:
- Tokenized Stocks
- Crypto Trading
- Self‑custody
- API Access
- Institutional Gateway
- On‑chain Liquidity
---
