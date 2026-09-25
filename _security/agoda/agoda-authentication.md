---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agoda-openapi-generated.yml
  format: yaml
  label: Agoda API
  slug: agoda-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agoda/refs/heads/main/openapi/_ae-authored/agoda-openapi-generated.yml
auth_types: []
description: Authentication methods for Agoda Direct Supply APIs
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Agoda Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agoda declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Agoda
provider_slug: agoda
scheme_count: 2
schemes:
- evidence: 'To obtain an access token, you need to call the following URL endpoint: URL ENDPOINT: https://supply.agoda.com/token-based-authentication/exchange'
  flows:
  - client_credentials
  how_to_obtain: Generate a Client ID and Client Secret in the API access management page in YCS, then call the token endpoint with those credentials to receive an access token.
  name: OAuth 2.0
  token_url: https://supply.agoda.com/token-based-authentication/exchange
  type: oauth2
- evidence: Both API Key authentication and Token-Based Authentication (OAuth 2.0) will be supported.
  name: API Key
  type: apiKey
slug: agoda-authentication
source_filename: agoda-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.agoda.com/supply/docs/authentication-2025
source_yaml: "generated: '2026-09-22'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.agoda.com/supply/docs/authentication-2025\nsources:\n- https://developer.agoda.com/supply/docs/authentication-2025\n- https://developer.agoda.com/supply/docs/getting-started\n- https://developer.agoda.com/supply/docs/setup-a-promotion-discount-with-different-nighttypes\ndescription: Authentication methods for Agoda Direct Supply APIs\nschemes:\n- type: oauth2\n  name: OAuth 2.0\n  evidence: 'To obtain an access token, you need to call the following URL endpoint: URL ENDPOINT: https://supply.agoda.com/token-based-authentication/exchange'\n  flows:\n  - client_credentials\n  token_url: https://supply.agoda.com/token-based-authentication/exchange\n  how_to_obtain: Generate a Client ID and Client Secret in the API access management page in YCS, then call the token endpoint with those credentials\n    to receive an access token.\n- type: apiKey\n  name: API Key\n  evidence:\
  \ Both API Key authentication and Token-Based Authentication (OAuth 2.0) will be supported.\ndocs: https://developer.agoda.com/supply/docs/authentication-2025\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agoda/refs/heads/main/authentication/agoda-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Travel
- Booking
- Hotels
- Online
---
