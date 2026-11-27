---
anonymous_access: false
api_key_in: []
api_specs:
- filename: gojinko-com-openapi-generated.yml
  format: yaml
  label: Jinko API
  slug: gojinko-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gojinko-com/openapi/_ae-authored/gojinko-com-openapi-generated.yml
auth_types: []
description: Authentication methods for Jinko as documented.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Jinko Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jinko declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Jinko
provider_slug: gojinko-com
scheme_count: 2
schemes:
- evidence: 'The REST API accepts both `X-API-Key: jnk_t_...` and `Authorization: Bearer jnk_t_...`; see [Which header to send].'
  header: X-API-Key
  how_to_obtain: Create a key in the dashboard or via an AI coding agent using `get_api_key`.
  location: header
  name: API Key
  type: apiKey
- evidence: MCP OAuth is the simplest option for end‑user‑facing MCP clients. The client discovers Jinko's authorization server, registers itself, and runs OAuth 2.1 with PKCE in the user's browser.
  how_to_obtain: The client registers dynamically with Jinko's authorization server (discovered at https://mcp.builders.gojinko.com/.well-known/oauth-authorization-server) and receives a client ID and secret.
  name: MCP OAuth (Dynamic Client Registration)
  type: oauth2
slug: gojinko-com-authentication
source_filename: gojinko-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.gojinko.com/authentication/api-keys.md
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.gojinko.com/authentication/api-keys.md\nsources:\n- https://docs.gojinko.com/authentication/api-keys.md\n- https://docs.gojinko.com/authentication/oauth.md\n- https://docs.gojinko.com/authentication/agent-registration.md\ndescription: Authentication methods for Jinko as documented.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'The REST API accepts both `X-API-Key: jnk_t_...` and `Authorization: Bearer jnk_t_...`; see [Which header to send].'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create a key in the dashboard or via an AI coding agent using `get_api_key`.\n- type: oauth2\n  name: MCP OAuth (Dynamic Client Registration)\n  evidence: MCP OAuth is the simplest option for end‑user‑facing MCP clients. The client discovers Jinko's authorization server, registers itself,\n    and runs OAuth 2.1 with PKCE in the user's browser.\n  how_to_obtain:\
  \ The client registers dynamically with Jinko's authorization server (discovered at https://mcp.builders.gojinko.com/.well-known/oauth-authorization-server)\n    and receives a client ID and secret.\ndocs: https://docs.gojinko.com/authentication/api-keys.md\n"
source_yaml_url: https://artifacts.apis.io/gojinko-com/authentication/gojinko-com-authentication.yml
summary_line: 2 schemes
tags:
- Travel
- Booking
- Agents
- Infrastructure
- Flights
- Hotels
- Car Rentals
---
