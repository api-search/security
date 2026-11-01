---
anonymous_access: false
api_key_in: []
api_specs:
- filename: useclad-ai-openapi-generated.yml
  format: yaml
  label: Clad Labs API
  slug: useclad-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/useclad-ai/openapi/_ae-authored/useclad-ai-openapi-generated.yml
auth_types: []
description: Authentication methods for Clad APIs
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Useclad Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clad Labs declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Clad Labs
provider_slug: useclad-ai
scheme_count: 2
schemes:
- evidence: 'Keys look like `clad_mk_...` and are passed as a Bearer token:'
  header: Authorization
  how_to_obtain: Create an API key in Settings → API (org admins only) and copy the `clad_mk_...` secret.
  location: header
  name: API Key
  type: http-bearer
- evidence: Clad runs a full **OAuth 2.1** authorization server — PKCE, dynamic client registration, refresh-token rotation with reuse detection, and RFC 8707 resource audiencing — the flow your client drives automatically.
  how_to_obtain: Add the server to a client (e.g., Cursor, Claude) and complete the sign‑in prompt; the client performs the OAuth authorization code flow with PKCE automatically.
  name: OAuth 2.1
  type: oauth2
slug: useclad-ai-authentication
source_filename: useclad-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.useclad.ai/api/authentication.md
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.useclad.ai/api/authentication.md\nsources:\n- https://docs.useclad.ai/api/authentication.md\n- https://docs.useclad.ai/api/reference-api-keys.md\n- https://docs.useclad.ai/mcp/connect-agent.md\n- https://docs.useclad.ai/mcp/connect-service.md\ndescription: Authentication methods for Clad APIs\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'Keys look like `clad_mk_...` and are passed as a Bearer token:'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in Settings → API (org admins only) and copy the `clad_mk_...` secret.\n- type: oauth2\n  name: OAuth 2.1\n  evidence: Clad runs a full **OAuth 2.1** authorization server — PKCE, dynamic client registration, refresh-token rotation with reuse detection,\n    and RFC 8707 resource audiencing — the flow your client drives automatically.\n  how_to_obtain: Add the server to a client\
  \ (e.g., Cursor, Claude) and complete the sign‑in prompt; the client performs the OAuth authorization\n    code flow with PKCE automatically.\ndocs: https://docs.useclad.ai/api/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/useclad-ai/authentication/useclad-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI
- Support
- SaaS
- Automation
---
