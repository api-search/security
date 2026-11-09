---
anonymous_access: false
api_key_in: []
api_specs:
- filename: actuallycare-com-v1-openapi.json
  format: json
  label: ActuallyCare API V1 API
  slug: actuallycare-api-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actuallycare-com/openapi/_original/actuallycare-com-v1-openapi.json
auth_types: []
description: Authentication methods for ActuallyCare API
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Actuallycare Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: ActuallyCare declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: ActuallyCare
provider_slug: actuallycare-com
scheme_count: 3
schemes:
- evidence: 'Most integrations authenticate with an API key in the `X-API-Key` header:'
  header: X-API-Key
  how_to_obtain: Create a key in the app under Settings → API Keys or via `POST /v1/api-keys` (requires a JWT).
  location: header
  name: API Key
  type: apiKey
- evidence: 'Send the access token on requests as a bearer token:'
  header: Authorization
  how_to_obtain: Log in via `POST /v1/auth/login` with email/username and password to receive an `accessToken`.
  location: header
  name: JWT Bearer Token
  token_url: https://api.actuallycare.com/v1/auth/login
  type: http-bearer
- evidence: When you add ActuallyCare as a connector in Claude, Claude starts an OAuth 2.1 flow with PKCE.
  how_to_obtain: OAuth flow is handled by Claude; no direct URLs are published in the documentation.
  name: OAuth 2.1 (Claude connector)
  type: oauth2
slug: actuallycare-com-authentication
source_filename: actuallycare-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.actuallycare.com/api/authentication.md
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.actuallycare.com/api/authentication.md\nsources:\n- https://docs.actuallycare.com/api/authentication.md\n- https://docs.actuallycare.com/api/reference/api-keys.md\n- https://docs.actuallycare.com/api/reference/authentication.md\n- https://docs.actuallycare.com/concepts/authentication.md\ndescription: Authentication methods for ActuallyCare API\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'Most integrations authenticate with an API key in the `X-API-Key` header:'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create a key in the app under Settings → API Keys or via `POST /v1/api-keys` (requires a JWT).\n- type: http-bearer\n  name: JWT Bearer Token\n  evidence: 'Send the access token on requests as a bearer token:'\n  location: header\n  header: Authorization\n  token_url: https://api.actuallycare.com/v1/auth/login\n  how_to_obtain: Log in via\
  \ `POST /v1/auth/login` with email/username and password to receive an `accessToken`.\n- type: oauth2\n  name: OAuth 2.1 (Claude connector)\n  evidence: When you add ActuallyCare as a connector in Claude, Claude starts an OAuth 2.1 flow with PKCE.\n  how_to_obtain: OAuth flow is handled by Claude; no direct URLs are published in the documentation.\ndocs: https://docs.actuallycare.com/api/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/actuallycare-com/authentication/actuallycare-com-authentication.yml
summary_line: 3 schemes
tags:
- Real Estate CRM
- AI Assistant
- Deal Tracking
- Partner Network
---
