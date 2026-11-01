---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mammoth-la-openapi-generated.yml
  format: yaml
  label: Mammoth Media API
  slug: mammoth-la-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mammoth-la/openapi/_ae-authored/mammoth-la-openapi-generated.yml
auth_types: []
description: Authentication methods published on the TokenBot documentation pages.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Mammoth La Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mammoth Media declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Mammoth Media
provider_slug: mammoth-la
scheme_count: 3
schemes:
- evidence: 'Send your API key via the `X-API-Key` header:'
  header: X-API-Key
  how_to_obtain: Create and manage keys with the CLI (`tokenbot apikey create ...`) or via the REST endpoints that require an ADMIN‑permission key.
  location: header
  name: X-API-Key
  type: apiKey
- evidence: 'You can also pass the same key as a bearer token — it''s treated identically:'
  header: Authorization
  how_to_obtain: Create and manage keys with the CLI (`tokenbot apikey create ...`) or via the REST endpoints that require an ADMIN‑permission key.
  location: header
  name: Authorization
  type: http-bearer
- evidence: The `tokenbot` CLI authenticates with a **secp256k1 keypair** instead of an API key. Each request carries four headers and a signature; no key is transmitted.
  how_to_obtain: Generated automatically by the `@tokenbot-org/cli-core` library; the client holds a secp256k1 private key and the CLI adds the required `x-tb-pubkey`, `x-tb-timestamp`, `x-tb-nonce`, and `x-tb-sig` headers.
  location: header
  name: Signed Request (CLI fast‑path)
  type: other
slug: mammoth-la-authentication
source_filename: mammoth-la-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.tokenbot.com/home/api-docs/authentication.md
source_yaml: "generated: '2026-10-26'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.tokenbot.com/home/api-docs/authentication.md\nsources:\n- https://docs.tokenbot.com/home/api-docs/authentication.md\n- https://docs.tokenbot.com/home/api-docs/rest-api/api-keys.md\n- https://docs.tokenbot.com/home/api-docs/quickstart.md\ndescription: Authentication methods published on the TokenBot documentation pages.\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: 'Send your API key via the `X-API-Key` header:'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create and manage keys with the CLI (`tokenbot apikey create ...`) or via the REST endpoints that require an ADMIN‑permission\n    key.\n- type: http-bearer\n  name: Authorization\n  evidence: 'You can also pass the same key as a bearer token — it''s treated identically:'\n  location: header\n  header: Authorization\n  how_to_obtain: Create and manage keys with the CLI (`tokenbot apikey create\
  \ ...`) or via the REST endpoints that require an ADMIN‑permission\n    key.\n- type: other\n  name: Signed Request (CLI fast‑path)\n  evidence: The `tokenbot` CLI authenticates with a **secp256k1 keypair** instead of an API key. Each request carries four headers and a signature;\n    no key is transmitted.\n  location: header\n  how_to_obtain: Generated automatically by the `@tokenbot-org/cli-core` library; the client holds a secp256k1 private key and the CLI adds the\n    required `x-tb-pubkey`, `x-tb-timestamp`, `x-tb-nonce`, and `x-tb-sig` headers.\ndocs: https://docs.tokenbot.com/home/api-docs/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/mammoth-la/authentication/mammoth-la-authentication.yml
summary_line: 3 schemes
tags:
- Crypto Trading
- Social Trading
- Token Utility
- Community Platform
---
