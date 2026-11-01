---
anonymous_access: false
api_key_in: []
api_specs:
- filename: vezgo-vezgo-api-openapi.yml
  format: yaml
  label: Vezgo API
  slug: vezgo-api-2
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vezgo/openapi/vezgo-vezgo-api-openapi.yml
- filename: vezgo-openapi-generated.yml
  format: yaml
  label: Vezgo API
  slug: vezgo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vezgo/openapi/_ae-authored/vezgo-openapi-generated.yml
auth_types: []
description: Authentication is required for user data endpoints in the form of a Vezgo user token.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Vezgo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vezgo declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Vezgo
provider_slug: vezgo
scheme_count: 1
schemes:
- evidence: 'The token must be included in the Authorization: Bearer ${token} header in your Vezgo API request, or in the ?token= query string in the Vezgo Connect widget URL.'
  header: Authorization
  how_to_obtain: POST to {VEZGO_API_URL}/auth/token with clientId and secret in the JSON body and the user's unique identifier passed as the loginName request header.
  location: header
  name: Bearer
  token_url: '{VEZGO_API_URL}/auth/token'
  type: http-bearer
slug: vezgo-authentication
source_filename: vezgo-authentication.yml
source_heading: Authentication Profile
source_url: https://vezgo.com/docs/authentication/
source_yaml: "generated: '2026-10-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://vezgo.com/docs/authentication/\nsources:\n- https://vezgo.com/docs/authentication/\n- https://vezgo.com/docs/api-management/\n- https://vezgo.com/docs/changelog/2026/08/08/wealthsimple-crypto-oauth/\n- https://vezgo.com/docs/changelog/2026/07/21/okx-oauth/\ndescription: Authentication is required for user data endpoints in the form of a Vezgo user token.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'The token must be included in the Authorization: Bearer ${token} header in your Vezgo API request, or in the ?token= query string\n    in the Vezgo Connect widget URL.'\n  location: header\n  header: Authorization\n  token_url: '{VEZGO_API_URL}/auth/token'\n  how_to_obtain: POST to {VEZGO_API_URL}/auth/token with clientId and secret in the JSON body and the user's unique identifier passed as the loginName\n    request header.\ndocs: https://vezgo.com/docs/authentication/\n"
source_yaml_url: https://artifacts.apis.io/vezgo/authentication/vezgo-authentication.yml
summary_line: 1 scheme
tags:
- Cryptocurrency
- Data API
- Digital Assets
- Fintech
- Portfolio Tracking
---
