---
anonymous_access: false
api_key_in: []
api_specs:
- filename: kinetune-com-v1-openapi.json
  format: json
  label: Kinetune API V1 API
  slug: kinetune-api-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kinetune-com/openapi/_original/kinetune-com-v1-openapi.json
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Kinetune Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kinetune declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Kinetune
provider_slug: kinetune-com
scheme_count: 2
schemes:
- evidence: 'Header Copy Text Authorization : Bearer kt_live_YOUR_KEY'
  header: Authorization
  how_to_obtain: Create one in Settings → Developer in the app (owners and admins). The secret is shown once; we store only an HMAC.
  location: header
  name: API Key
  type: apiKey
- authorize_url: /api/auth/oauth2/authorize
  evidence: 'OAuth 2.1: authorization code with PKCE (S256), dynamic client registration and client ID metadata documents, rotating refresh tokens.'
  how_to_obtain: Sign in with the app — MCP clients and the CLI. Connected apps are listed in Settings → Developer, where each can be disconnected.
  name: OAuth 2.1
  scopes:
  - videos:read
  - videos:write
  - music:read
  - music:write
  - library:read
  - library:write
  - organizations:read
  - organizations:write
  token_url: /api/auth/oauth2/token
  type: oauth2
slug: kinetune-com-authentication
source_filename: kinetune-com-authentication.yml
source_heading: Authentication Profile
source_url: https://kinetune.com/developers/authentication
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://kinetune.com/developers/authentication\nsources:\n- https://kinetune.com/developers/authentication\n- https://kinetune.com/developers/rest\n- https://kinetune.com/developers/quickstart\ndescription: Authentication\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'Header Copy Text Authorization : Bearer kt_live_YOUR_KEY'\n  location: header\n  header: Authorization\n  how_to_obtain: Create one in Settings → Developer in the app (owners and admins). The secret is shown once; we store only an HMAC.\n- type: oauth2\n  name: OAuth 2.1\n  evidence: 'OAuth 2.1: authorization code with PKCE (S256), dynamic client registration and client ID metadata documents, rotating refresh tokens.'\n  token_url: /api/auth/oauth2/token\n  authorize_url: /api/auth/oauth2/authorize\n  scopes:\n  - videos:read\n  - videos:write\n  - music:read\n  - music:write\n  - library:read\n  - library:write\n\
  \  - organizations:read\n  - organizations:write\n  how_to_obtain: Sign in with the app — MCP clients and the CLI. Connected apps are listed in Settings → Developer, where each can be disconnected.\ndocs: https://kinetune.com/developers/authentication\n"
source_yaml_url: https://artifacts.apis.io/kinetune-com/authentication/kinetune-com-authentication.yml
summary_line: 2 schemes
tags:
- Music
- Artificial Intelligence
- Video
- Software-as-a-Service
- Media
---
