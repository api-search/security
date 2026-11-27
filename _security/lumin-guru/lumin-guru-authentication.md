---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lumin-guru-openapi-generated.yml
  format: yaml
  label: Lumin API
  slug: lumin-guru-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumin-guru/openapi/_ae-authored/lumin-guru-openapi-generated.yml
auth_types: []
description: 'Lumin supports two authentication modes: API key and OAuth 2.1.'
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Lumin Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lumin declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Lumin
provider_slug: lumin-guru
scheme_count: 1
schemes:
- evidence: 'An API key goes in as Authorization: Bearer mcp_... .'
  header: Authorization
  how_to_obtain: Generate a key at https://app.lumin.guru/api-keys.
  location: header
  name: API Key
  type: apiKey
slug: lumin-guru-authentication
source_filename: lumin-guru-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.lumin.guru/build/guides/api-key-vs-oauth
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.lumin.guru/build/guides/api-key-vs-oauth\nsources:\n- https://docs.lumin.guru/build/guides/api-key-vs-oauth\n- https://docs.lumin.guru/build/reference/auth\n- https://docs.lumin.guru/build/reference/tools/find-contract-signing-time\n- https://docs.lumin.guru/build/quickstart\ndescription: 'Lumin supports two authentication modes: API key and OAuth 2.1.'\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'An API key goes in as Authorization: Bearer mcp_... .'\n  location: header\n  header: Authorization\n  how_to_obtain: Generate a key at https://app.lumin.guru/api-keys.\ndocs: https://docs.lumin.guru/build/guides/api-key-vs-oauth\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/lumin-guru/authentication/lumin-guru-authentication.yml
summary_line: 1 scheme
tags:
- Astrology
- Artificial Intelligence
- Compute
- MCP
- Trust
---
