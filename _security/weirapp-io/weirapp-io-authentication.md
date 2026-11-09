---
anonymous_access: false
api_key_in: []
api_specs:
- filename: weirapp-io-account-api-openapi.yml
  format: yaml
  label: weirapp-io Account API
  slug: weirapp-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/weirapp-io/openapi/weirapp-io-account-api-openapi.yml
- filename: weirapp-io-monitors-api-openapi.yml
  format: yaml
  label: weirapp-io Monitors API
  slug: weirapp-io-monitors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/weirapp-io/openapi/weirapp-io-monitors-api-openapi.yml
- filename: weirapp-io-reddit-api-openapi.yml
  format: yaml
  label: weirapp-io Reddit API
  slug: weirapp-io-reddit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/weirapp-io/openapi/weirapp-io-reddit-api-openapi.yml
- filename: weirapp-io-system-api-openapi.yml
  format: yaml
  label: weirapp-io System API
  slug: weirapp-io-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/weirapp-io/openapi/weirapp-io-system-api-openapi.yml
- filename: weirapp-io-webhooks-api-openapi.yml
  format: yaml
  label: weirapp-io Webhooks API
  slug: weirapp-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/weirapp-io/openapi/weirapp-io-webhooks-api-openapi.yml
- filename: weirapp-io-x-api-openapi.yml
  format: yaml
  label: weirapp-io X API
  slug: weirapp-io-x-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/weirapp-io/openapi/weirapp-io-x-api-openapi.yml
auth_types: []
description: Authentication methods for Weir API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Weirapp Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: weirapp-io declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: weirapp-io
provider_slug: weirapp-io
scheme_count: 2
schemes:
- evidence: 'One header, on every request: Authorization: Bearer weir_live_...'
  header: Authorization
  how_to_obtain: Create keys under API keys. A key is shown once, when you create it.
  location: header
  name: Authorization
  type: http-bearer
- evidence: Claude, ChatGPT, Cursor, and most coding agents connect to https://api.weirapp.io/mcp with OAuth 2.1.
  how_to_obtain: Clients register themselves, by dynamic client registration or a Client ID Metadata Document, so there is no client ID to paste. Every client is public (no secret) and must use PKCE with S256.
  name: OAuth2
  scopes:
  - read:reddit
  - read:x
  - read:social
  - usage:read
  - monitors:read
  - monitors:write
  - webhooks:read
  - webhooks:write
  type: oauth2
slug: weirapp-io-authentication
source_filename: weirapp-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.weirapp.io/authentication
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.weirapp.io/authentication\nsources:\n- https://docs.weirapp.io/authentication\n- https://docs.weirapp.io/agent-setup\n- https://docs.weirapp.io/quickstart\ndescription: Authentication methods for Weir API\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: 'One header, on every request: Authorization: Bearer weir_live_...'\n  location: header\n  header: Authorization\n  how_to_obtain: Create keys under API keys. A key is shown once, when you create it.\n- type: oauth2\n  name: OAuth2\n  evidence: Claude, ChatGPT, Cursor, and most coding agents connect to https://api.weirapp.io/mcp with OAuth 2.1.\n  scopes:\n  - read:reddit\n  - read:x\n  - read:social\n  - usage:read\n  - monitors:read\n  - monitors:write\n  - webhooks:read\n  - webhooks:write\n  how_to_obtain: Clients register themselves, by dynamic client registration or a Client ID Metadata Document,\
  \ so there is no client ID to paste.\n    Every client is public (no secret) and must use PKCE with S256.\ndocs: https://docs.weirapp.io/authentication\n"
source_yaml_url: https://artifacts.apis.io/weirapp-io/authentication/weirapp-io-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Data
- Social Media
- MCP
---
