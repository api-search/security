---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aspiresingapore-openapi-generated.yml
  format: yaml
  label: Aspiresingapore API
  slug: aspiresingapore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aspiresingapore/refs/heads/main/openapi/_ae-authored/aspiresingapore-openapi-generated.yml
auth_types: []
description: Authentication methods for Aspire API
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Aspiresingapore Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aspiresingapore declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Aspiresingapore
provider_slug: aspiresingapore
scheme_count: 3
schemes:
- evidence: 'Every Aspire API request must be authenticated with an access token , sent as a bearer token in the Authorization header:'
  header: Authorization
  how_to_obtain: 'Obtain an access token via one of the supported authentication flows and include it as "Authorization: Bearer {access_token}" on each request.'
  location: header
  name: Bearer token
  type: http-bearer
- evidence: 'Method 1 — API Key (client credentials)​ Create an API key in the Aspire dashboard and securely store the Client ID and Client Secret (the secret is shown only once). Exchange them for an access token:'
  header: Authorization
  how_to_obtain: Create an API key in the Aspire dashboard, then POST to the token endpoint with grant_type=client_credentials, client_id and client_secret to receive an access token.
  location: header
  name: API Key (client credentials)
  token_url: https://api.aspireapp.com/public/v1/login
  type: oauth2
- authorize_url: https://app.aspireapp.com/oauth/connect?client_id=<CLIENT_ID>&redirect_uri=<REDIRECT_URI>&...
  evidence: 'Method 2 — OAuth 2.0 (Authorization Code + PKCE)​ For third‑party apps acting on a user''s behalf, Aspire uses the Authorization Code flow with PKCE:'
  header: Authorization
  how_to_obtain: Register your app to receive a client ID, redirect the user to the authorization URL, then exchange the returned authorization code for an access token (and refresh token).
  location: header
  name: OAuth 2.0 (Authorization Code + PKCE)
  type: oauth2
slug: aspiresingapore-authentication
source_filename: aspiresingapore-authentication.yml
source_heading: Authentication Profile
source_url: https://help.aspireapp.com/en/articles/9285867-how-to-set-up-a-biometric-authentication.md
source_yaml: "generated: '2026-09-26'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://help.aspireapp.com/en/articles/9285867-how-to-set-up-a-biometric-authentication.md\nsources:\n- https://help.aspireapp.com/en/articles/9285867-how-to-set-up-a-biometric-authentication.md\n- https://docs.api.aspireapp.com/authentication\n- https://help.aspireapp.com/en/articles/15433833-getting-started.md\ndescription: Authentication methods for Aspire API\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Every Aspire API request must be authenticated with an access token , sent as a bearer token in the Authorization header:'\n  location: header\n  header: Authorization\n  how_to_obtain: 'Obtain an access token via one of the supported authentication flows and include it as \"Authorization: Bearer {access_token}\"\n    on each request.'\n- type: oauth2\n  name: API Key (client credentials)\n  evidence: 'Method 1 — API Key (client credentials)​ Create an API\
  \ key in the Aspire dashboard and securely store the Client ID and Client Secret\n    (the secret is shown only once). Exchange them for an access token:'\n  location: header\n  header: Authorization\n  token_url: https://api.aspireapp.com/public/v1/login\n  how_to_obtain: Create an API key in the Aspire dashboard, then POST to the token endpoint with grant_type=client_credentials, client_id and\n    client_secret to receive an access token.\n- type: oauth2\n  name: OAuth 2.0 (Authorization Code + PKCE)\n  evidence: 'Method 2 — OAuth 2.0 (Authorization Code + PKCE)​ For third‑party apps acting on a user''s behalf, Aspire uses the Authorization\n    Code flow with PKCE:'\n  location: header\n  header: Authorization\n  authorize_url: https://app.aspireapp.com/oauth/connect?client_id=<CLIENT_ID>&redirect_uri=<REDIRECT_URI>&...\n  how_to_obtain: Register your app to receive a client ID, redirect the user to the authorization URL, then exchange the returned authorization\n    code for an access\
  \ token (and refresh token).\ndocs: https://help.aspireapp.com/en/articles/9285867-how-to-set-up-a-biometric-authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aspiresingapore/refs/heads/main/authentication/aspiresingapore-authentication.yml
summary_line: 3 schemes
tags:
- Finance
- Banking
- API
- Singapore
- SaaS
---
