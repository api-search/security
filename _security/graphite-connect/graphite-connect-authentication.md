---
anonymous_access: false
api_key_in: []
api_specs:
- filename: graphite-connect-oauth-api-openapi.yml
  format: yaml
  label: Graphite Connect OAuth API
  slug: graphite-connect-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/graphite-connect/refs/heads/main/openapi/graphite-connect-oauth-api-openapi.yml
- filename: graphite-connect-profile-api-openapi.yml
  format: yaml
  label: Graphite Connect Profile API
  slug: graphite-connect-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/graphite-connect/refs/heads/main/openapi/graphite-connect-profile-api-openapi.yml
- filename: graphite-connect-search-api-openapi.yml
  format: yaml
  label: Graphite Connect Search API
  slug: graphite-connect-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/graphite-connect/refs/heads/main/openapi/graphite-connect-search-api-openapi.yml
auth_types: []
description: Graphite Connect Public API uses OAuth 2.0 client credentials flow to obtain a bearer token, which is then sent in the Authorization header.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Graphite Connect Authentication
name_suffix: Authentication
oauth_flows: []
overview: Graphite Connect declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Graphite Connect
provider_slug: graphite-connect
scheme_count: 2
schemes:
- evidence: The Graphite Connect Public API uses **OAuth 2.0 client credentials** flow.
  flows:
  - client_credentials
  how_to_obtain: Contact support@graphiteconnect.com to get an API key, which serves as both client ID and client secret, then POST to the token endpoint with grant_type=client_credentials.
  name: OAuth 2.0 Client Credentials
  token_url: https://app.graphiteconnect.com/api/oauth/token
  type: oauth2
- evidence: 'Include the bearer token in the `Authorization` header of all subsequent API requests:'
  header: Authorization
  how_to_obtain: Exchange the API key for a bearer token via the OAuth token endpoint.
  name: Bearer Token
  type: http-bearer
slug: graphite-connect-authentication
source_filename: graphite-connect-authentication.yml
source_heading: Authentication Profile
source_url: https://apidocs.graphiteconnect.com/docs/authentication.md
source_yaml: "generated: '2026-10-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://apidocs.graphiteconnect.com/docs/authentication.md\nsources:\n- https://apidocs.graphiteconnect.com/docs/authentication.md\n- https://apidocs.graphiteconnect.com/reference/authentication.md\n- https://apidocs.graphiteconnect.com/reference/authentication\n- https://apidocs.graphiteconnect.com/docs/authentication\ndescription: Graphite Connect Public API uses OAuth 2.0 client credentials flow to obtain a bearer token, which is then sent in the Authorization\n  header.\nschemes:\n- type: oauth2\n  name: OAuth 2.0 Client Credentials\n  evidence: The Graphite Connect Public API uses **OAuth 2.0 client credentials** flow.\n  flows:\n  - client_credentials\n  token_url: https://app.graphiteconnect.com/api/oauth/token\n  how_to_obtain: Contact support@graphiteconnect.com to get an API key, which serves as both client ID and client secret, then POST to the token\n    endpoint with\
  \ grant_type=client_credentials.\n- type: http-bearer\n  name: Bearer Token\n  evidence: 'Include the bearer token in the `Authorization` header of all subsequent API requests:'\n  header: Authorization\n  how_to_obtain: Exchange the API key for a bearer token via the OAuth token endpoint.\ndocs: https://apidocs.graphiteconnect.com/docs/authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/graphite-connect/refs/heads/main/authentication/graphite-connect-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Supplier Management
- Procurement
- Artificial Intelligence
- Risk Management
---
