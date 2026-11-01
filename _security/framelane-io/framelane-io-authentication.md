---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for Framelane API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Framelane Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: framelane-io declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: framelane-io
provider_slug: framelane-io
scheme_count: 1
schemes:
- evidence: All API requests require a Bearer API key.
  header: Authorization
  how_to_obtain: Create and manage API keys in the console under Settings → API Keys, or self‑provision via POST /v1/signup → POST /v1/signup/verify.
  location: header
  name: Bearer API key
  type: http-bearer
slug: framelane-io-authentication
source_filename: framelane-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.framelane.io/introduction/authentication.md
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.framelane.io/introduction/authentication.md\nsources:\n- https://docs.framelane.io/introduction/authentication.md\n- https://docs.framelane.io/api-reference/api-keys/create-api-key.md\n- https://docs.framelane.io/api-reference/api-keys/list-api-keys.md\n- https://docs.framelane.io/api-reference/api-keys/revoke-api-key.md\ndescription: Authentication schemes for Framelane API\nschemes:\n- type: http-bearer\n  name: Bearer API key\n  evidence: All API requests require a Bearer API key.\n  location: header\n  header: Authorization\n  how_to_obtain: Create and manage API keys in the console under Settings → API Keys, or self‑provision via POST /v1/signup → POST /v1/signup/verify.\nnote: No OAuth2 or other authentication schemes are documented.\ndocs: https://docs.framelane.io/introduction/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/framelane-io/authentication/framelane-io-authentication.yml
summary_line: 1 scheme
tags:
- Video Editing
- Rendering API
- AI Agents
- GPU Rendering
- Video Production
- SDK
---
