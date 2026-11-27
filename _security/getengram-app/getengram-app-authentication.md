---
anonymous_access: false
api_key_in: []
api_specs:
- filename: getengram-app-openapi-generated.yml
  format: yaml
  label: Engram API
  slug: getengram-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getengram-app/openapi/_ae-authored/getengram-app-openapi-generated.yml
auth_types: []
description: Engram uses API keys passed as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Engram Authentication
name_suffix: Authentication
oauth_flows: []
overview: Engram declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Engram
provider_slug: getengram-app
scheme_count: 1
schemes:
- evidence: 'Pass your API key in the Authorization header: Authorization: Bearer engram_sk_live_your_key_here'
  header: Authorization
  how_to_obtain: Create an account with `engram signup` (or `engram login` if you already have an account) which returns a key shown once on creation.
  location: header
  name: Authorization
  type: apiKey
slug: getengram-app-authentication
source_filename: getengram-app-authentication.yml
source_heading: Authentication Profile
source_url: https://getengram.app/docs/authentication
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://getengram.app/docs/authentication\nsources:\n- https://getengram.app/docs/authentication\n- https://getengram.app/docs/getting-started\ndescription: Engram uses API keys passed as a Bearer token in the Authorization header.\nschemes:\n- type: apiKey\n  name: Authorization\n  evidence: 'Pass your API key in the Authorization header: Authorization: Bearer engram_sk_live_your_key_here'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an account with `engram signup` (or `engram login` if you already have an account) which returns a key shown once on creation.\nnote: Engram does not document any OAuth2, http‑basic, http‑bearer, JWT, HMAC, mTLS, or other authentication flows.\ndocs: https://getengram.app/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/getengram-app/authentication/getengram-app-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Memory
- Agents
- MCP
- Storage
- Company
---
