---
api_key_in:
- header
- query
api_specs:
- filename: ocean-io-autocomplete-api-openapi.yml
  format: yaml
  label: Ocean.io Autocomplete API
  slug: ocean-io-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocean-io/refs/heads/main/openapi/ocean-io-autocomplete-api-openapi.yml
- filename: ocean-io-enrich-api-openapi.yml
  format: yaml
  label: Ocean.io Enrich API
  slug: ocean-io-enrich-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocean-io/refs/heads/main/openapi/ocean-io-enrich-api-openapi.yml
- filename: ocean-io-lookup-api-openapi.yml
  format: yaml
  label: Ocean.io Lookup API
  slug: ocean-io-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocean-io/refs/heads/main/openapi/ocean-io-lookup-api-openapi.yml
- filename: ocean-io-ocean-io-api-documentation-api-openapi.yml
  format: yaml
  label: Ocean.io Ocean.io API Documentation API
  slug: ocean-io-ocean-io-api-documentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocean-io/refs/heads/main/openapi/ocean-io-ocean-io-api-documentation-api-openapi.yml
- filename: ocean-io-other-api-openapi.yml
  format: yaml
  label: Ocean.io Other API
  slug: ocean-io-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocean-io/refs/heads/main/openapi/ocean-io-other-api-openapi.yml
- filename: ocean-io-reveal-api-openapi.yml
  format: yaml
  label: Ocean.io Reveal API
  slug: ocean-io-reveal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocean-io/refs/heads/main/openapi/ocean-io-reveal-api-openapi.yml
- filename: ocean-io-search-api-openapi.yml
  format: yaml
  label: Ocean.io Search API
  slug: ocean-io-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocean-io/refs/heads/main/openapi/ocean-io-search-api-openapi.yml
- filename: ocean-io-segmentation-api-openapi.yml
  format: yaml
  label: Ocean.io Segmentation API
  slug: ocean-io-segmentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocean-io/refs/heads/main/openapi/ocean-io-segmentation-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: Ocean.io authenticates every REST call with a single account API token, generated in the app under Account Settings → API tokens. The token may be sent either as the X-Api-Token request header or as an apiToken query parameter — but not both, which is an error. There are no scopes and no per-token permissions surface documented. The published OpenAPI does not declare components.securitySchemes; instead every one of the 26 operations carries the token as two optional parameters (apiToken in query, x-api-token in header), so a generated client will not enforce auth. A separate RFC 8414 OAuth 2.0 Authorization Server Metadata document is served at https://api.ocean.io/.well-known/oauth-authorization-server advertising a client_credentials token endpoint; it is not referenced anywhere in the public documentation.
kind: authentication
layout: security
method: searched
name: Ocean Io Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Ocean.io secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Ocean.io
provider_slug: ocean-io
scheme_count: 3
schemes:
- description: Preferred method. Headers do not appear in server logs or browser history, which the docs give as the reason to prefer it over the query parameter.
  example_request: 'curl -X GET ''https://api.ocean.io/v2/credits/balance'' -H ''X-Api-Token: YOUR_API_TOKEN'''
  in: header
  name: X-Api-Token
  parameter: X-Api-Token
  primary: true
  recommended: true
  sources:
  - https://app.ocean.io/docs/getting-started/authentication
  - openapi/ocean-io-api-openapi.yml
  type: apiKey
- description: Alternative method; the same token passed as a query-string parameter.
  example_request: curl -X GET 'https://api.ocean.io/v2/credits/balance?apiToken=YOUR_API_TOKEN'
  in: query
  name: apiToken
  parameter: apiToken
  primary: false
  recommended: false
  sources:
  - https://app.ocean.io/docs/getting-started/authentication
  - openapi/ocean-io-api-openapi.yml
  type: apiKey
- description: Discovered only from the RFC 8414 metadata document at https://api.ocean.io/.well-known/oauth-authorization-server (HTTP 200, application/json). No Ocean.io documentation page describes this flow, no client registration process is published, and scopes_supported is empty.
  documented: false
  flow: clientCredentials
  issuer: https://api.ocean.io
  name: OAuth 2.0 client credentials
  scopes_supported: []
  sources:
  - well-known/ocean-io-oauth-authorization-server.json
  token_endpoint_auth_methods_supported:
  - client_secret_post
  token_url: https://api.ocean.io/oauth/token
  type: oauth2
slug: ocean-io-authentication
source_filename: ocean-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/ocean-io-api-openapi.yml + well-known/ocean-io-oauth-authorization-server.json\ndocs: https://app.ocean.io/docs/getting-started/authentication\ndescription: >-\n  Ocean.io authenticates every REST call with a single account API token, generated in the app under\n  Account Settings → API tokens. The token may be sent either as the X-Api-Token request header or as\n  an apiToken query parameter — but not both, which is an error. There are no scopes and no per-token\n  permissions surface documented. The published OpenAPI does not declare components.securitySchemes;\n  instead every one of the 26 operations carries the token as two optional parameters (apiToken in\n  query, x-api-token in header), so a generated client will not enforce auth. A separate RFC 8414\n  OAuth 2.0 Authorization Server Metadata document is served at\n  https://api.ocean.io/.well-known/oauth-authorization-server advertising a client_credentials\
  \ token\n  endpoint; it is not referenced anywhere in the public documentation.\nsummary:\n  types:\n    - apiKey\n    - oauth2\n  api_key_in:\n    - header\n    - query\n  oauth2_flows:\n    - clientCredentials\n  scopes_declared: 0\n  openapi_security_schemes_declared: 0\nschemes:\n  - name: X-Api-Token\n    type: apiKey\n    in: header\n    parameter: X-Api-Token\n    primary: true\n    recommended: true\n    description: >-\n      Preferred method. Headers do not appear in server logs or browser history, which the docs give\n      as the reason to prefer it over the query parameter.\n    example_request: \"curl -X GET 'https://api.ocean.io/v2/credits/balance' -H 'X-Api-Token: YOUR_API_TOKEN'\"\n    sources:\n      - https://app.ocean.io/docs/getting-started/authentication\n      - openapi/ocean-io-api-openapi.yml\n  - name: apiToken\n    type: apiKey\n    in: query\n    parameter: apiToken\n    primary: false\n    recommended: false\n    description: Alternative method; the same token\
  \ passed as a query-string parameter.\n    example_request: \"curl -X GET 'https://api.ocean.io/v2/credits/balance?apiToken=YOUR_API_TOKEN'\"\n    sources:\n      - https://app.ocean.io/docs/getting-started/authentication\n      - openapi/ocean-io-api-openapi.yml\n  - name: OAuth 2.0 client credentials\n    type: oauth2\n    flow: clientCredentials\n    token_url: https://api.ocean.io/oauth/token\n    issuer: https://api.ocean.io\n    token_endpoint_auth_methods_supported:\n      - client_secret_post\n    scopes_supported: []\n    documented: false\n    description: >-\n      Discovered only from the RFC 8414 metadata document at\n      https://api.ocean.io/.well-known/oauth-authorization-server (HTTP 200, application/json). No\n      Ocean.io documentation page describes this flow, no client registration process is published,\n      and scopes_supported is empty.\n    sources:\n      - well-known/ocean-io-oauth-authorization-server.json\ntoken_errors:\n  - scenario: Token missing from\
  \ request\n    status: 403\n    body: '{\"detail\": \"API token should be provided in headers or query parameters\"}'\n  - scenario: Token is invalid or unrecognised\n    status: 403\n    body: '{\"detail\": \"Invalid API token\"}'\n  - scenario: Token provided in both header and query parameter\n    status: 400\n    body: '{\"detail\": \"Conflicting API tokens provided in query parameters and headers\"}'\nrotation:\n  supported: true\n  process: >-\n    Revoke a suspected-compromised token immediately in Account Settings and generate a new one;\n    update all consuming systems before revoking to avoid downtime.\n  docs: https://app.ocean.io/docs/getting-started/authentication\nmcp:\n  endpoint: https://api.ocean.io/mcp/\n  auth: same account API token, passed as the api-token query parameter on the endpoint URL\ngaps:\n  - >-\n    The OpenAPI declares no components.securitySchemes and no security requirement, so the auth\n    contract is only discoverable from prose. Declaring an apiKey\
  \ scheme (header X-Api-Token) and\n    applying it globally would make the spec self-describing for generated clients and agents.\n  - >-\n    The OAuth authorization-server metadata is published but undocumented; a consumer cannot obtain\n    client credentials from any public page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ocean-io/refs/heads/main/authentication/ocean-io-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Sales Intelligence
- B2B
- Enrichment
- Lookalike
- ABM
- Prospecting
- Company Data
- People Data
- Contact Data
- Segmentation
- Go-To-Market
- MCP
---
