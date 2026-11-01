---
anonymous_access: false
api_key_in: []
api_specs:
- filename: memxus-com-openapi-generated.yml
  format: yaml
  label: memxus-com API
  slug: memxus-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memxus-com/openapi/_ae-authored/memxus-com-openapi-generated.yml
auth_types: []
description: Memxus supports OAuth (one‑click Google sign‑in) and Bearer token authentication using an API key.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Memxus Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: memxus-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: memxus-com
provider_slug: memxus-com
scheme_count: 2
schemes:
- authorize_url: https://dashboard.memxus.com/oauth/authorize
  evidence: One‑click OAuth install — no API keys to copy. Click Connect with One Click (works on phone, tablet, or computer).
  flows:
  - authorization_code
  how_to_obtain: Sign in with Google via the connection hub when prompted.
  name: One‑Click OAuth
  type: oauth2
- evidence: 'Bearer fallback (Cursor): create an API key in dashboard.memxus.com → API Keys , then Settings → MCP → Add new MCP server.'
  header: Authorization
  how_to_obtain: Copy the aimem_* key from https://dashboard.memxus.com/api-keys after first login.
  location: header
  name: Bearer API Key
  type: http-bearer
slug: memxus-com-authentication
source_filename: memxus-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.memxus.com/docs/getting-started
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.memxus.com/docs/getting-started\nsources:\n- https://www.memxus.com/docs/getting-started\n- https://www.memxus.com/docs/mcp\ndescription: Memxus supports OAuth (one‑click Google sign‑in) and Bearer token authentication using an API key.\nschemes:\n- type: oauth2\n  name: One‑Click OAuth\n  evidence: One‑click OAuth install — no API keys to copy. Click Connect with One Click (works on phone, tablet, or computer).\n  flows:\n  - authorization_code\n  authorize_url: https://dashboard.memxus.com/oauth/authorize\n  how_to_obtain: Sign in with Google via the connection hub when prompted.\n- type: http-bearer\n  name: Bearer API Key\n  evidence: 'Bearer fallback (Cursor): create an API key in dashboard.memxus.com → API Keys , then Settings → MCP → Add new MCP server.'\n  location: header\n  header: Authorization\n  how_to_obtain: Copy the aimem_* key from https://dashboard.memxus.com/api-keys\
  \ after first login.\ndocs: https://www.memxus.com/docs/getting-started\n"
source_yaml_url: https://artifacts.apis.io/memxus-com/authentication/memxus-com-authentication.yml
summary_line: 2 schemes
tags:
- AI
- ContextEngine
- DeveloperTools
- Productivity
- Memory
---
