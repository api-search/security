---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication for lurq API uses an API key sent as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: lurq Authentication
name_suffix: Authentication
oauth_flows: []
overview: lurq declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: lurq
provider_slug: lurq-run
scheme_count: 1
schemes:
- evidence: 'Every entry points at https://api.lurq.run/mcp and sends Authorization: Bearer <your-key> .'
  header: Authorization
  how_to_obtain: Create a key on Dashboard → API keys.
  location: header
  name: Bearer
  type: http-bearer
slug: lurq-run-authentication
source_filename: lurq-run-authentication.yml
source_heading: Authentication Profile
source_url: https://www.lurq.run/docs/quickstart
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.lurq.run/docs/quickstart\nsources:\n- https://www.lurq.run/docs/quickstart\ndescription: Authentication for lurq API uses an API key sent as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Every entry points at https://api.lurq.run/mcp and sends Authorization: Bearer <your-key> .'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key on Dashboard → API keys.\nnote: No OAuth2 flows, API key is the only authentication method described.\ndocs: https://www.lurq.run/docs/quickstart\n"
source_yaml_url: https://artifacts.apis.io/lurq-run/authentication/lurq-run-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- npm
- Package Security
- Verification
- Developer Tools
---
