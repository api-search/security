---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dealroom-api-openapi.yml
  format: yaml
  label: Dealroom API API
  slug: dealroom-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealroom/refs/heads/main/openapi/_original/dealroom-api-openapi.yml
auth_types: []
description: Dealroom API authentication
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Dealroom Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dealroom declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Dealroom
provider_slug: dealroom
scheme_count: 2
schemes:
- evidence: The Dealroom API uses API keys for server-side integrations. Each key has a `client_id` and `client_secret` and uses the OAuth2 client credentials grant.
  flows:
  - client_credentials
  how_to_obtain: Create an API key in the Dealroom dashboard (Settings → Developer → API keys) which provides a `client_id` and `client_secret`. Then exchange them for a Bearer token at the token endpoint using the client_credentials grant.
  name: Dealroom OAuth2 Client Credentials
  token_url: https://accounts.dealroom.co/oauth/token
  type: oauth2
- evidence: Safe to share, and sent on every request as the `X-Client-Id` header.
  header: X-Client-Id
  how_to_obtain: Use the `client_id` from the API key created in the Dealroom dashboard.
  location: header
  name: X-Client-Id header
  type: apiKey
slug: dealroom-authentication
source_filename: dealroom-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.dealroom.co/getting-started/authentication.md
source_yaml: "generated: '2026-10-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.dealroom.co/getting-started/authentication.md\nsources:\n- https://developers.dealroom.co/getting-started/authentication.md\n- https://developers.dealroom.co/getting-started/quickstart.md\n- https://developers.dealroom.co/getting-started/agent-setup.md\ndescription: Dealroom API authentication\nschemes:\n- type: oauth2\n  name: Dealroom OAuth2 Client Credentials\n  evidence: The Dealroom API uses API keys for server-side integrations. Each key has a `client_id` and `client_secret` and uses the OAuth2 client\n    credentials grant.\n  flows:\n  - client_credentials\n  token_url: https://accounts.dealroom.co/oauth/token\n  how_to_obtain: Create an API key in the Dealroom dashboard (Settings → Developer → API keys) which provides a `client_id` and `client_secret`.\n    Then exchange them for a Bearer token at the token endpoint using the client_credentials grant.\n\
  - type: apiKey\n  name: X-Client-Id header\n  evidence: Safe to share, and sent on every request as the `X-Client-Id` header.\n  location: header\n  header: X-Client-Id\n  how_to_obtain: Use the `client_id` from the API key created in the Dealroom dashboard.\ndocs: https://developers.dealroom.co/getting-started/authentication.md\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dealroom/refs/heads/main/authentication/dealroom-authentication.yml
summary_line: 2 schemes
tags:
- Company
---
