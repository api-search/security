---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: OpenComment AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenComment AI declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: OpenComment AI
provider_slug: opencomment-ai
scheme_count: 2
schemes:
- evidence: Provide the key through your client's secure credential settings or an environment variable as a bearer token.
  header: Authorization
  how_to_obtain: Create a named API key in OpenComment account settings under Agent access; the key is displayed once and can be set via an environment variable or private header.
  location: header
  name: API Key
  type: http-bearer
- evidence: The OAuth issuer is `https://api.opencomment.ai/auth`; discovery uses standard metadata and authorization-code sign-in with PKCE.
  how_to_obtain: Run the client’s OAuth sign‑in flow (e.g., codex mcp login, Claude connector sign‑in, or Cursor OAuth action) to obtain an authorization code and exchange it for a token.
  name: OAuth
  type: oauth2
slug: opencomment-ai-authentication
source_filename: opencomment-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://opencomment.ai/mcp/quickstart.md
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://opencomment.ai/mcp/quickstart.md\nsources:\n- https://opencomment.ai/mcp/quickstart.md\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: Provide the key through your client's secure credential settings or an environment variable as a bearer token.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a named API key in OpenComment account settings under Agent access; the key is displayed once and can be set via an environment\n    variable or private header.\n- type: oauth2\n  name: OAuth\n  evidence: The OAuth issuer is `https://api.opencomment.ai/auth`; discovery uses standard metadata and authorization-code sign-in with PKCE.\n  how_to_obtain: Run the client’s OAuth sign‑in flow (e.g., codex mcp login, Claude connector sign‑in, or Cursor OAuth action) to obtain an authorization\n    code and exchange it for a token.\ndocs: https://opencomment.ai/mcp/quickstart.md\n"
source_yaml_url: https://artifacts.apis.io/opencomment-ai/authentication/opencomment-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Sales
- Marketing
- Outreach
- Artificial Intelligence
---
