---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods as published on the Ragfeed developer page.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Ragfeed De Authentication
name_suffix: Authentication
oauth_flows: []
overview: ragfeed-de declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ragfeed-de
provider_slug: ragfeed-de
scheme_count: 2
schemes:
- evidence: 'Authenticate with Authorization: Bearer sk-… – keys always start with sk-.'
  header: Authorization
  how_to_obtain: Get a key by signing up at /signup; the key is shown once and never sent by e‑mail.
  location: header
  name: Bearer token
  type: http-bearer
- evidence: Claude / any MCP client https://api.ragfeed.de/mcp , OAuth 2.1 with dynamic client registration, or your API key as Bearer.
  name: OAuth 2.1
  type: oauth2
slug: ragfeed-de-authentication
source_filename: ragfeed-de-authentication.yml
source_heading: Authentication Profile
source_url: https://ragfeed.de/en/developers
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://ragfeed.de/en/developers\nsources:\n- https://ragfeed.de/en/developers\ndescription: Authentication methods as published on the Ragfeed developer page.\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Authenticate with Authorization: Bearer sk-… – keys always start with sk-.'\n  location: header\n  header: Authorization\n  how_to_obtain: Get a key by signing up at /signup; the key is shown once and never sent by e‑mail.\n- type: oauth2\n  name: OAuth 2.1\n  evidence: Claude / any MCP client https://api.ragfeed.de/mcp , OAuth 2.1 with dynamic client registration, or your API key as Bearer.\ndocs: https://ragfeed.de/en/developers\n"
source_yaml_url: https://artifacts.apis.io/ragfeed-de/authentication/ragfeed-de-authentication.yml
summary_line: 2 schemes
tags:
- Web Scraping
- API
- AI Data
- EU Hosting
- Compliance
- SaaS
---
