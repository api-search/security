---
anonymous_access: false
api_key_in: []
api_specs:
- filename: frontlatch-com-tools-api-openapi.yml
  format: yaml
  label: Frontlatch Tools API
  slug: frontlatch-com-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/frontlatch-com/openapi/frontlatch-com-tools-api-openapi.yml
auth_types: []
description: Frontlatch supports optional API‑key authentication and OAuth 2.1 with PKCE for authenticated access.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Frontlatch Authentication
name_suffix: Authentication
oauth_flows: []
overview: Frontlatch declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Frontlatch
provider_slug: frontlatch-com
scheme_count: 2
schemes:
- evidence: An optional key from /app/developer can be created and revoked. A call that carries a valid key is counted against the key instead of the session, at 500 requests an hour, and is attributed to you.
  how_to_obtain: Create a key in the Frontlatch developer portal at /app/developer.
  name: optional API key
  type: apiKey
- authorize_url: /.well-known/oauth-authorization-server
  evidence: It is OAuth 2.1 with PKCE and the AI registers itself, so there is nothing to copy. Without a token, /mcp/auth answers 401 and points at /.well-known/oauth-protected-resource/mcp/auth ; the sign-in server is described at /.well-known/oauth-authorization-server.
  flows:
  - authorization_code
  how_to_obtain: Perform the OAuth 2.1 authorization code flow with PKCE as described by the server’s .well-known endpoints.
  name: Frontlatch OAuth 2.1 with PKCE
  type: oauth2
slug: frontlatch-com-authentication
source_filename: frontlatch-com-authentication.yml
source_heading: Authentication Profile
source_url: https://frontlatch.com/docs/developer-quickstart
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://frontlatch.com/docs/developer-quickstart\nsources:\n- https://frontlatch.com/docs/developer-quickstart\ndescription: Frontlatch supports optional API‑key authentication and OAuth 2.1 with PKCE for authenticated access.\nschemes:\n- type: apiKey\n  name: optional API key\n  evidence: An optional key from /app/developer can be created and revoked. A call that carries a valid key is counted against the key instead\n    of the session, at 500 requests an hour, and is attributed to you.\n  how_to_obtain: Create a key in the Frontlatch developer portal at /app/developer.\n- type: oauth2\n  name: Frontlatch OAuth 2.1 with PKCE\n  evidence: It is OAuth 2.1 with PKCE and the AI registers itself, so there is nothing to copy. Without a token, /mcp/auth answers 401 and points\n    at /.well-known/oauth-protected-resource/mcp/auth ; the sign-in server is described at /.well-known/oauth-authorization-server.\n\
  \  flows:\n  - authorization_code\n  authorize_url: /.well-known/oauth-authorization-server\n  how_to_obtain: Perform the OAuth 2.1 authorization code flow with PKCE as described by the server’s .well-known endpoints.\ndocs: https://frontlatch.com/docs/developer-quickstart\n"
source_yaml_url: https://artifacts.apis.io/frontlatch-com/authentication/frontlatch-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- Booking
- Small Business
- Automation
---
