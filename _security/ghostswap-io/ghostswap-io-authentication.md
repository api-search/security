---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication uses a Bearer token composed of the public key and secret joined by a colon.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: GhostSwap Authentication
name_suffix: Authentication
oauth_flows: []
overview: GhostSwap declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: GhostSwap
provider_slug: ghostswap-io
scheme_count: 1
schemes:
- evidence: 'Every request to /v1/* requires an Authorization: Bearer header. The token is your public key and secret , joined by a single colon.'
  header: Authorization
  location: header
  name: Bearer
  type: http-bearer
slug: ghostswap-io-authentication
source_filename: ghostswap-io-authentication.yml
source_heading: Authentication Profile
source_url: https://partners.ghostswap.io/docs/auth
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://partners.ghostswap.io/docs/auth\nsources:\n- https://partners.ghostswap.io/docs/auth\n- https://partners.ghostswap.io/docs/quickstart\ndescription: Authentication uses a Bearer token composed of the public key and secret joined by a colon.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Every request to /v1/* requires an Authorization: Bearer header. The token is your public key and secret , joined by a single colon.'\n  location: header\n  header: Authorization\nnote: The token is formed as <public_key>:<secret> and placed in the Authorization header as \"Bearer <public_key>:<secret>\".\ndocs: https://partners.ghostswap.io/docs/auth\n"
source_yaml_url: https://artifacts.apis.io/ghostswap-io/authentication/ghostswap-io-authentication.yml
summary_line: 1 scheme
tags:
- Cryptocurrency
- Exchange
- Anonymous
- NoKYC
- Swap
---
