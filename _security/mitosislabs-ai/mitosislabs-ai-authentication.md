---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Mitosis Labs APIs
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Mitosis Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mitosis Labs declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Mitosis Labs
provider_slug: mitosislabs-ai
scheme_count: 2
schemes:
- evidence: 'Send the credential as an HTTP `Authorization` header. `header` is the only `bearer_methods_supported` value advertised by the protected-resource metadata:'
  header: Authorization
  how_to_obtain: Create a key in the dashboard (Copy API Key) or run `mi login` which stores an `mi_`‑prefixed key in `~/.os1/config.json`.
  location: header
  name: API Key / JWT
  type: http-bearer
- evidence: 'For humans at a terminal, the CLI runs a device-code flow: it prints a URL, you approve in the browser, and the session is stored locally.'
  how_to_obtain: Run `mi login` which initiates the device‑code flow, or register dynamically via the OAuth 2.1 discovery endpoint `https://mitosislabs.ai/.well-known/oauth-authorization-server`.
  name: Device‑code flow (OAuth 2.1)
  scopes:
  - memory:read
  - memory:write
  - backups:read
  - backups:write
  - backups:admin
  - openid
  - profile
  - email
  type: oauth2
slug: mitosislabs-ai-authentication
source_filename: mitosislabs-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://mitosislabs.ai/developers/authentication
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mitosislabs.ai/developers/authentication\nsources:\n- https://mitosislabs.ai/developers/authentication\n- https://mitosislabs.ai/auth.md\n- https://mitosislabs.ai/backups/llms.txt\n- https://mitosislabs.ai/developers/quickstart\ndescription: Authentication methods for Mitosis Labs APIs\nschemes:\n- type: http-bearer\n  name: API Key / JWT\n  evidence: 'Send the credential as an HTTP `Authorization` header. `header` is the only `bearer_methods_supported` value advertised by the protected-resource\n    metadata:'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in the dashboard (Copy API Key) or run `mi login` which stores an `mi_`‑prefixed key in `~/.os1/config.json`.\n- type: oauth2\n  name: Device‑code flow (OAuth 2.1)\n  evidence: 'For humans at a terminal, the CLI runs a device-code flow: it prints a URL, you approve in the browser, and the\
  \ session is stored\n    locally.'\n  scopes:\n  - memory:read\n  - memory:write\n  - backups:read\n  - backups:write\n  - backups:admin\n  - openid\n  - profile\n  - email\n  how_to_obtain: Run `mi login` which initiates the device‑code flow, or register dynamically via the OAuth 2.1 discovery endpoint `https://mitosislabs.ai/.well-known/oauth-authorization-server`.\ndocs: https://mitosislabs.ai/developers/authentication\n"
source_yaml_url: https://artifacts.apis.io/mitosislabs-ai/authentication/mitosislabs-ai-authentication.yml
summary_line: 2 schemes
tags:
- AI Agents
- Enterprise AI
- Privacy
---
