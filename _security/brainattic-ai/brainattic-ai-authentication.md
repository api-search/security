---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for brainattic
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Brainattic Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: brainattic declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: brainattic
provider_slug: brainattic-ai
scheme_count: 1
schemes:
- evidence: brainattic uses OAuth 2.1 — the same secure sign-in standard your client already uses for its other connectors.
  flows:
  - authorization_code
  how_to_obtain: Each person signs in with their own brainattic account the first time they use it, and approves access.
  name: OAuth 2.1
  scopes:
  - brainattic:access
  type: oauth2
slug: brainattic-ai-authentication
source_filename: brainattic-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://brainattic.ai/docs/auth
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://brainattic.ai/docs/auth\nsources:\n- https://brainattic.ai/docs/auth\n- https://brainattic.ai/docs/quickstart\ndescription: Authentication schemes for brainattic\nschemes:\n- type: oauth2\n  name: OAuth 2.1\n  evidence: brainattic uses OAuth 2.1 — the same secure sign-in standard your client already uses for its other connectors.\n  flows:\n  - authorization_code\n  scopes:\n  - brainattic:access\n  how_to_obtain: Each person signs in with their own brainattic account the first time they use it, and approves access.\ndocs: https://brainattic.ai/docs/auth\n"
source_yaml_url: https://artifacts.apis.io/brainattic-ai/authentication/brainattic-ai-authentication.yml
summary_line: 1 scheme
tags:
- Knowledge Base
- Artificial Intelligence
- Enterprise
- Governance
- MCP
- Company
---
