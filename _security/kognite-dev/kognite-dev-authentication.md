---
anonymous_access: false
api_key_in: []
api_specs:
- filename: kognite-dev-openapi-generated.yml
  format: yaml
  label: Kognite API
  slug: kognite-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kognite-dev/openapi/_ae-authored/kognite-dev-openapi-generated.yml
auth_types: []
description: Authentication methods for Kognite as described on the Quickstart page.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Kognite Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kognite declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Kognite
provider_slug: kognite-dev
scheme_count: 2
schemes:
- evidence: Kognite speaks the standard MCP Streamable HTTP transport and implements the MCP authorization flow (OAuth 2.1 with PKCE and dynamic client registration).
  flows:
  - authorization_code
  how_to_obtain: The client opens a browser tab where the user signs in or creates a free account and approves the connection; the client then receives a short‑lived token that it refreshes automatically.
  name: MCP authorization flow
  type: oauth2
- evidence: Prefer to paste a key instead? For a client that can’t do the browser handshake, create a key at app.kognite.dev under Connect and put it in the URL instead.
  how_to_obtain: Create a key at app.kognite.dev under Connect and insert it into the URL as https://mcp.kognite.dev/t/YOUR_KEY.
  location: url
  name: Bearer key in URL
  type: apiKey
slug: kognite-dev-authentication
source_filename: kognite-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://kognite.dev/docs/quickstart
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://kognite.dev/docs/quickstart\nsources:\n- https://kognite.dev/docs/quickstart\ndescription: Authentication methods for Kognite as described on the Quickstart page.\nschemes:\n- type: oauth2\n  name: MCP authorization flow\n  evidence: Kognite speaks the standard MCP Streamable HTTP transport and implements the MCP authorization flow (OAuth 2.1 with PKCE and dynamic\n    client registration).\n  flows:\n  - authorization_code\n  how_to_obtain: The client opens a browser tab where the user signs in or creates a free account and approves the connection; the client then\n    receives a short‑lived token that it refreshes automatically.\n- type: apiKey\n  name: Bearer key in URL\n  evidence: Prefer to paste a key instead? For a client that can’t do the browser handshake, create a key at app.kognite.dev under Connect and\n    put it in the URL instead.\n  location: url\n  how_to_obtain:\
  \ Create a key at app.kognite.dev under Connect and insert it into the URL as https://mcp.kognite.dev/t/YOUR_KEY.\ndocs: https://kognite.dev/docs/quickstart\n"
source_yaml_url: https://artifacts.apis.io/kognite-dev/authentication/kognite-dev-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- Memory
- Platform
- MCP
---
