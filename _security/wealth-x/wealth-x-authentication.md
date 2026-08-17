---
api_key_in:
- header
api_specs:
- filename: wealth-x-dossiers-api-openapi.yml
  format: yaml
  label: Wealth-X Dossiers API
  slug: wealth-x-dossiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wealth-x/refs/heads/main/openapi/wealth-x-dossiers-api-openapi.yml
- filename: wealth-x-reference-api-openapi.yml
  format: yaml
  label: Wealth-X Reference API
  slug: wealth-x-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wealth-x/refs/heads/main/openapi/wealth-x-reference-api-openapi.yml
- filename: wealth-x-search-api-openapi.yml
  format: yaml
  label: Wealth-X Search API
  slug: wealth-x-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wealth-x/refs/heads/main/openapi/wealth-x-search-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: Three distinct authentication models across the Wealth-X / Altrata estate. The legacy Wealth-X Connect REST API uses three static credential headers. The successor Altrata GraphQL APIs use an OAuth 2.0 client_credentials token exchange that itself requires an API key plus HTTP Basic service credentials. The Altrata MCP server uses OAuth 2.0 authorization_code with PKCE.
kind: authentication
layout: security
method: searched
name: Wealth X Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wealth-X secures its APIs with apiKey, http, and oauth2 across 7 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Wealth-X
provider_slug: wealth-x
scheme_count: 7
schemes:
- description: Wealth-X account username, supplied as a request header.
  in: header
  method: derived
  name: wealthxUsername
  parameter: username
  sources:
  - openapi/wealth-x-dossiers-api-openapi.yml
  - openapi/wealth-x-reference-api-openapi.yml
  - openapi/wealth-x-search-api-openapi.yml
  surface: Wealth-X Connect REST API (legacy)
  type: apiKey
- description: Wealth-X account password, supplied as a request header.
  in: header
  method: derived
  name: wealthxPassword
  parameter: password
  sources:
  - openapi/wealth-x-dossiers-api-openapi.yml
  - openapi/wealth-x-reference-api-openapi.yml
  - openapi/wealth-x-search-api-openapi.yml
  surface: Wealth-X Connect REST API (legacy)
  type: apiKey
- description: Wealth-X API key, supplied as a request header.
  in: header
  method: derived
  name: wealthxApiKey
  parameter: apikey
  sources:
  - openapi/wealth-x-dossiers-api-openapi.yml
  - openapi/wealth-x-reference-api-openapi.yml
  - openapi/wealth-x-search-api-openapi.yml
  surface: Wealth-X Connect REST API (legacy)
  type: apiKey
- caution: The Altrata service-user username is NOT the account email — it is the username sent during initial password setup.
  description: 'POST to the Altrata token endpoint with an `x-api-key` header carrying the subscription API key and an `Authorization: Basic base64(username:password)` header carrying the service user credentials. The returned access token is then presented on the GraphQL call.'
  flow: clientCredentials
  grant_type_in: query string (?grant_type=client_credentials)
  method: searched
  name: altrataServiceToken
  scopes: []
  scopes_note: No scope parameter or scope list is documented for this flow.
  source: https://docs.altrata.com/service-user-credentials
  surface: Altrata platform GraphQL APIs
  token_url: https://api.auth.altrata.com/oauth2/token
  type: oauth2
- description: Subscription API key, required on the token request in addition to the service user's HTTP Basic credentials. Also the key used by the Altrata Salesforce App.
  in: header
  method: searched
  name: altrataApiKey
  parameter: x-api-key
  source: https://docs.altrata.com/service-user-credentials
  surface: Altrata platform GraphQL APIs
  type: apiKey
- description: base64(serviceUsername:servicePassword) on the token request.
  method: searched
  name: altrataBasic
  scheme: basic
  source: https://docs.altrata.com/service-user-credentials
  surface: Altrata platform GraphQL APIs (token request)
  type: http
- authorization_url: https://serviceauth.altrata.com/oauth2/authorize
  client_id: 21saqug474pjtpong1gue9505
  description: 'Amazon Cognito-backed OAuth. An anonymous request returns HTTP 401 with a spec-conformant challenge — WWW-Authenticate: Bearer realm="Altrata MCP", resource_metadata=".../.well-known/oauth-protected-resource/mcp", scope="openid email".'
  detail: scopes/wealth-x-scopes.yml
  flow: authorizationCode
  grant_types_supported:
  - authorization_code
  - refresh_token
  issuer: https://mcp.altrata.com
  jwks_uri: https://cognito-idp.us-east-2.amazonaws.com/us-east-2_Pe8aMS8JG/.well-known/jwks.json
  method: probed
  name: altrataMcpOAuth
  pkce: S256
  scopes:
  - openid
  - email
  surface: Altrata MCP server (https://mcp.altrata.com/mcp)
  token_endpoint_auth_methods_supported:
  - none
  token_url: https://serviceauth.altrata.com/oauth2/token
  type: oauth2
slug: wealth-x-authentication
source_filename: wealth-x-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: >-\n  https://docs.altrata.com/service-user-credentials and\n  https://mcp.altrata.com/.well-known/oauth-authorization-server (searched/probed);\n  openapi/wealth-x-*-openapi.yml (derived).\ndocs: https://docs.altrata.com/service-user-credentials\ndescription: >-\n  Three distinct authentication models across the Wealth-X / Altrata estate. The\n  legacy Wealth-X Connect REST API uses three static credential headers. The\n  successor Altrata GraphQL APIs use an OAuth 2.0 client_credentials token\n  exchange that itself requires an API key plus HTTP Basic service credentials.\n  The Altrata MCP server uses OAuth 2.0 authorization_code with PKCE.\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  self_serve: false\n  provisioning_note: >-\n    No self-serve signup for any surface. Credentials are issued by email during\n    subscription setup; missing credentials go to clientsuccess@altrata.com\
  \ or a\n    client success representative.\n\nschemes:\n- name: wealthxUsername\n  surface: Wealth-X Connect REST API (legacy)\n  type: apiKey\n  in: header\n  parameter: username\n  description: Wealth-X account username, supplied as a request header.\n  method: derived\n  sources:\n  - openapi/wealth-x-dossiers-api-openapi.yml\n  - openapi/wealth-x-reference-api-openapi.yml\n  - openapi/wealth-x-search-api-openapi.yml\n- name: wealthxPassword\n  surface: Wealth-X Connect REST API (legacy)\n  type: apiKey\n  in: header\n  parameter: password\n  description: Wealth-X account password, supplied as a request header.\n  method: derived\n  sources:\n  - openapi/wealth-x-dossiers-api-openapi.yml\n  - openapi/wealth-x-reference-api-openapi.yml\n  - openapi/wealth-x-search-api-openapi.yml\n- name: wealthxApiKey\n  surface: Wealth-X Connect REST API (legacy)\n  type: apiKey\n  in: header\n  parameter: apikey\n  description: Wealth-X API key, supplied as a request header.\n  method: derived\n \
  \ sources:\n  - openapi/wealth-x-dossiers-api-openapi.yml\n  - openapi/wealth-x-reference-api-openapi.yml\n  - openapi/wealth-x-search-api-openapi.yml\n- name: altrataServiceToken\n  surface: Altrata platform GraphQL APIs\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://api.auth.altrata.com/oauth2/token\n  grant_type_in: query string (?grant_type=client_credentials)\n  description: >-\n    POST to the Altrata token endpoint with an `x-api-key` header carrying the\n    subscription API key and an `Authorization: Basic base64(username:password)`\n    header carrying the service user credentials. The returned access token is\n    then presented on the GraphQL call.\n  method: searched\n  caution: >-\n    The Altrata service-user username is NOT the account email — it is the\n    username sent during initial password setup.\n  scopes: []\n  scopes_note: No scope parameter or scope list is documented for this flow.\n  source: https://docs.altrata.com/service-user-credentials\n\
  - name: altrataApiKey\n  surface: Altrata platform GraphQL APIs\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: >-\n    Subscription API key, required on the token request in addition to the\n    service user's HTTP Basic credentials. Also the key used by the Altrata\n    Salesforce App.\n  method: searched\n  source: https://docs.altrata.com/service-user-credentials\n- name: altrataBasic\n  surface: Altrata platform GraphQL APIs (token request)\n  type: http\n  scheme: basic\n  description: base64(serviceUsername:servicePassword) on the token request.\n  method: searched\n  source: https://docs.altrata.com/service-user-credentials\n- name: altrataMcpOAuth\n  surface: Altrata MCP server (https://mcp.altrata.com/mcp)\n  type: oauth2\n  flow: authorizationCode\n  pkce: S256\n  issuer: https://mcp.altrata.com\n  authorization_url: https://serviceauth.altrata.com/oauth2/authorize\n  token_url: https://serviceauth.altrata.com/oauth2/token\n  jwks_uri: https://cognito-idp.us-east-2.amazonaws.com/us-east-2_Pe8aMS8JG/.well-known/jwks.json\n\
  \  client_id: 21saqug474pjtpong1gue9505\n  token_endpoint_auth_methods_supported: [none]\n  grant_types_supported: [authorization_code, refresh_token]\n  scopes:\n  - openid\n  - email\n  description: >-\n    Amazon Cognito-backed OAuth. An anonymous request returns HTTP 401 with a\n    spec-conformant challenge — WWW-Authenticate: Bearer realm=\"Altrata MCP\",\n    resource_metadata=\".../.well-known/oauth-protected-resource/mcp\",\n    scope=\"openid email\".\n  method: probed\n  detail: scopes/wealth-x-scopes.yml\n\nhuman_access:\n  graphiql: >-\n    The GraphiQL explorers at <service>.altrata.com/v1/graphiql/ accept the\n    service account username and password directly in a sign-in form — no token\n    exchange needed for interactive use.\n  source: https://docs.altrata.com/service-user-credentials\n\ngaps:\n- No self-serve signup, trial, or public sandbox credential on any surface.\n- No openid-configuration document is served, despite the `openid` scope.\n- The legacy REST API\
  \ transmits an account password as a plain request header on every call.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wealth-x/refs/heads/main/authentication/wealth-x-authentication.yml
summary_line: apiKey/http/oauth2 · 7 schemes
tags:
- Company
- Wealth Intelligence
- Data
- UHNW
- Prospecting
- Financial Services
- CRM
- People Data
- Altrata
- GraphQL
- MCP
- Wealth Screening
---
