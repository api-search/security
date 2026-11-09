---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bugtape-ai-openapi-generated.yml
  format: yaml
  label: BugTape API
  slug: bugtape-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugtape-ai/openapi/_ae-authored/bugtape-ai-openapi-generated.yml
auth_types: []
description: Authentication methods for BugTape as documented.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Bugtape Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: BugTape declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: BugTape
provider_slug: bugtape-ai
scheme_count: 2
schemes:
- evidence: 'Pass the key in the X-BugTape-Key header:'
  header: X-BugTape-Key
  how_to_obtain: Keys are generated via the console or the POST /v1/projects/:id/keys endpoint.
  location: header
  name: API Key
  type: apiKey
- evidence: 'Access token : 1 hour expiry, passed as Authorization: Bearer <token> .'
  header: Authorization
  how_to_obtain: Console users authenticate with email/password and receive JWT tokens.
  location: header
  name: JWT
  type: http-bearer
slug: bugtape-ai-authentication
source_filename: bugtape-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://bugtape.ai/docs/authentication/
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://bugtape.ai/docs/authentication/\nsources:\n- https://bugtape.ai/docs/authentication/\n- https://bugtape.ai/docs/authentication/\n- https://bugtape.ai/docs/authentication.md\n- https://bugtape.ai/guides/unexpected-token-not-valid-json/\ndescription: Authentication methods for BugTape as documented.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'Pass the key in the X-BugTape-Key header:'\n  location: header\n  header: X-BugTape-Key\n  how_to_obtain: Keys are generated via the console or the POST /v1/projects/:id/keys endpoint.\n- type: http-bearer\n  name: JWT\n  evidence: 'Access token : 1 hour expiry, passed as Authorization: Bearer <token> .'\n  location: header\n  header: Authorization\n  how_to_obtain: Console users authenticate with email/password and receive JWT tokens.\ndocs: https://bugtape.ai/docs/authentication/\nnote: 1 extracted row(s) were dropped because\
  \ their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/bugtape-ai/authentication/bugtape-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Error Tracking
- AI Agents
- Developer Tools
- Software-as-a-Service
---
