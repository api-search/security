---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for PrompTessor as documented.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Promptessor Authentication
name_suffix: Authentication
oauth_flows: []
overview: PrompTessor declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: PrompTessor
provider_slug: promptessor
scheme_count: 1
schemes:
- authorize_url: https://auth.promptessor.com/authorize
  evidence: PrompTessor supports the authorization-code flow with PKCE S256, public clients with token endpoint authentication method none, refresh tokens, revocation, protected-resource metadata, authorization-server metadata, JWKS, and dynamic client registration.
  how_to_obtain: Register a public client via https://auth.promptessor.com/register (no client secret), then perform the PKCE authorization‑code flow as described.
  name: OAuth 2.0
  scopes:
  - prompts:generate
  - prompts:presets:read
  - prompts:presets:write
  - prompts:analyze
  - prompts:optimize
  - prompts:refine
  - prompts:reverse
  - uploads:write
  - usage:read
  - history:read
  - history:manage
  - library:read
  - library:write
  - library:interact
  - library:publish
  - operations:read
  - operations:cancel
  - webhooks:manage
  token_url: https://auth.promptessor.com/token
  type: oauth2
slug: promptessor-authentication
source_filename: promptessor-authentication.yml
source_heading: Authentication Profile
source_url: https://promptessor.com/dev/docs/authentication
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://promptessor.com/dev/docs/authentication\nsources:\n- https://promptessor.com/dev/docs/authentication\n- https://promptessor.com/dev/docs/mcp/integrations\n- https://promptessor.com/dev/docs/quickstart\ndescription: Authentication schemes for PrompTessor as documented.\nschemes:\n- type: oauth2\n  name: OAuth 2.0\n  evidence: PrompTessor supports the authorization-code flow with PKCE S256, public clients with token endpoint authentication method none, refresh\n    tokens, revocation, protected-resource metadata, authorization-server metadata, JWKS, and dynamic client registration.\n  token_url: https://auth.promptessor.com/token\n  authorize_url: https://auth.promptessor.com/authorize\n  scopes:\n  - prompts:generate\n  - prompts:presets:read\n  - prompts:presets:write\n  - prompts:analyze\n  - prompts:optimize\n  - prompts:refine\n  - prompts:reverse\n  - uploads:write\n\
  \  - usage:read\n  - history:read\n  - history:manage\n  - library:read\n  - library:write\n  - library:interact\n  - library:publish\n  - operations:read\n  - operations:cancel\n  - webhooks:manage\n  how_to_obtain: Register a public client via https://auth.promptessor.com/register (no client secret), then perform the PKCE authorization‑code\n    flow as described.\ndocs: https://promptessor.com/dev/docs/authentication\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/promptessor/authentication/promptessor-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Prompt Engineering
- Platform
- Documentation
- Community
---
