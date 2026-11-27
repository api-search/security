---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for EQVPS API/MCP
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: EQVPS Authentication
name_suffix: Authentication
oauth_flows: []
overview: EQVPS declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: EQVPS
provider_slug: eqvps-com
scheme_count: 1
schemes:
- evidence: EQVPS uses Bearer tokens — but there are two SEPARATE auth paths, do not mix them.
  header: Authorization
  how_to_obtain: 'Call register_account (or login) through the API/MCP to receive a token instantly; the token is then sent as Authorization: Bearer <token> on every request.'
  location: header
  name: Bearer token
  type: http-bearer
slug: eqvps-com-authentication
source_filename: eqvps-com-authentication.yml
source_heading: Authentication Profile
source_url: https://eqvps.com/en/docs/auth
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://eqvps.com/en/docs/auth\nsources:\n- https://eqvps.com/en/docs/auth\n- https://eqvps.com/en/wiki/how-to-set-up-ssh-key-authentication\n- https://eqvps.com/en/use-cases/vps-for-mcp-gateway\n- https://eqvps.com/en/wiki/agent-mcp-login\ndescription: Authentication schemes for EQVPS API/MCP\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: EQVPS uses Bearer tokens — but there are two SEPARATE auth paths, do not mix them.\n  location: header\n  header: Authorization\n  how_to_obtain: 'Call register_account (or login) through the API/MCP to receive a token instantly; the token is then sent as Authorization:\n    Bearer <token> on every request.'\nnote: Humans sign in via the website using OAuth or email OTP, but those flows are not documented on the API pages and thus are not included.\ndocs: https://eqvps.com/en/docs/auth\n"
source_yaml_url: https://artifacts.apis.io/eqvps-com/authentication/eqvps-com-authentication.yml
summary_line: 1 scheme
tags:
- Private
- VPS
- Cryptocurrency
- NoKYC
- EU
---
