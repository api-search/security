---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for BRONTIR MCP API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Brontir Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: BRONTIR declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: BRONTIR
provider_slug: brontir-com
scheme_count: 2
schemes:
- evidence: BRONTIR takes an API key from your account, sent as a bearer token. The key comes from your BRONTIR account.
  header: Authorization
  how_to_obtain: Create an API key on the API keys panel of your account.
  location: header
  name: API Key
  type: http-bearer
- evidence: Clients with OAuth support sign in with Google and need no key; their guides are on the other tabs.
  how_to_obtain: Sign in with Google through the client’s sign‑in flow.
  name: Google OAuth
  type: oauth2
slug: brontir-com-authentication
source_filename: brontir-com-authentication.yml
source_heading: Authentication Profile
source_url: https://brontir.com/setup/other-clients
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://brontir.com/setup/other-clients\nsources:\n- https://brontir.com/setup/other-clients\n- https://brontir.com/setup\n- https://brontir.com/setup/claude\ndescription: Authentication methods for BRONTIR MCP API\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: BRONTIR takes an API key from your account, sent as a bearer token. The key comes from your BRONTIR account.\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key on the API keys panel of your account.\n- type: oauth2\n  name: Google OAuth\n  evidence: Clients with OAuth support sign in with Google and need no key; their guides are on the other tabs.\n  how_to_obtain: Sign in with Google through the client’s sign‑in flow.\ndocs: https://brontir.com/setup/other-clients\n"
source_yaml_url: https://artifacts.apis.io/brontir-com/authentication/brontir-com-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Data Integration
- Web Research
- Public Data
- Software-as-a-Service
---
