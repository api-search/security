---
anonymous_access: false
api_key_in: []
api_specs:
- filename: frankki-app-openapi-generated.yml
  format: yaml
  label: FrankKi API
  slug: frankki-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/frankki-app/openapi/_ae-authored/frankki-app-openapi-generated.yml
auth_types: []
description: FrankKi supports OAuth 2.1 with PKCE for interactive clients and bearer API keys for headless clients.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: FrankKi Authentication
name_suffix: Authentication
oauth_flows: []
overview: FrankKi declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: FrankKi
provider_slug: frankki-app
scheme_count: 2
schemes:
- evidence: Interactive clients use OAuth 2.1 with PKCE (S256) and dynamic client registration (RFC 7591) at the remote MCP endpoint https://mcp.frankki.app.
  how_to_obtain: Open a browser to the sign‑in window or follow the OpenAI guide to authorize the client; the flow uses PKCE and dynamic client registration.
  name: OAuth 2.1 with PKCE
  type: oauth2
- evidence: 'Headless agents use a bearer API key issued at https://frankki.app/dashboard/tokens. Store it in a secret manager and send Authorization: Bearer <FRANKKI_API_KEY>.'
  header: Authorization
  how_to_obtain: Create a token at https://frankki.app/dashboard/tokens and copy the raw token shown once.
  location: header
  name: Bearer API key
  type: apiKey
slug: frankki-app-authentication
source_filename: frankki-app-authentication.yml
source_heading: Authentication Profile
source_url: https://frankki.app/en/developers/quickstart/chatgpt
source_yaml: "generated: '2026-11-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://frankki.app/en/developers/quickstart/chatgpt\nsources:\n- https://frankki.app/en/developers/quickstart/chatgpt\n- https://frankki.app/en/developers/agent-onboarding\n- https://frankki.app/en/developers/quickstart/cursor\n- https://frankki.app/en/developers/integrations/codex\ndescription: FrankKi supports OAuth 2.1 with PKCE for interactive clients and bearer API keys for headless clients.\nschemes:\n- type: oauth2\n  name: OAuth 2.1 with PKCE\n  evidence: Interactive clients use OAuth 2.1 with PKCE (S256) and dynamic client registration (RFC 7591) at the remote MCP endpoint https://mcp.frankki.app.\n  how_to_obtain: Open a browser to the sign‑in window or follow the OpenAI guide to authorize the client; the flow uses PKCE and dynamic client\n    registration.\n- type: apiKey\n  name: Bearer API key\n  evidence: 'Headless agents use a bearer API key issued at https://frankki.app/dashboard/tokens.\
  \ Store it in a secret manager and send Authorization:\n    Bearer <FRANKKI_API_KEY>.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a token at https://frankki.app/dashboard/tokens and copy the raw token shown once.\ndocs: https://frankki.app/en/developers/quickstart/chatgpt\n"
source_yaml_url: https://artifacts.apis.io/frankki-app/authentication/frankki-app-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- Automation
- Messaging
- Software-as-a-Service
---
