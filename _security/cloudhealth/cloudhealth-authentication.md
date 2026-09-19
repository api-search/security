---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: cloudhealth-aws-accounts-api-openapi.yml
  format: yaml
  label: CloudHealth AWS Accounts API
  slug: cloudhealth-aws-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudhealth/refs/heads/main/openapi/cloudhealth-aws-accounts-api-openapi.yml
- filename: cloudhealth-perspectives-api-openapi.yml
  format: yaml
  label: CloudHealth Perspectives API
  slug: cloudhealth-perspectives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudhealth/refs/heads/main/openapi/cloudhealth-perspectives-api-openapi.yml
- filename: cloudhealth-reports-api-openapi.yml
  format: yaml
  label: CloudHealth Reports API
  slug: cloudhealth-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudhealth/refs/heads/main/openapi/cloudhealth-reports-api-openapi.yml
- filename: cloudhealth-search-api-openapi.yml
  format: yaml
  label: CloudHealth Search API
  slug: cloudhealth-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudhealth/refs/heads/main/openapi/cloudhealth-search-api-openapi.yml
- filename: cloudhealth-sso-api-openapi.yml
  format: yaml
  label: CloudHealth SSO API
  slug: cloudhealth-sso-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudhealth/refs/heads/main/openapi/cloudhealth-sso-api-openapi.yml
auth_types:
- http
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Cloudhealth Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: CloudHealth secures its APIs with http, apiKey, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: CloudHealth
provider_slug: cloudhealth
scheme_count: 4
schemes:
- description: 'Per-user API key (a GUID generated under My Profile > API Key) sent as "Authorization: Bearer <api_key>". Every request must also send Accept: application/json (or Content-Type: application/json). Generating a new key invalidates the previous one; the docs recommend periodic rotation. The API enforces the same organization scoping and role restrictions as the CloudHealth UI.'
  evidence: https://apidocs.cloudhealthtech.com/#documentation_how-to-use-the-cloudhealth-api
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cloudhealth-aws-accounts-api-openapi.yml
  - openapi/cloudhealth-perspectives-api-openapi.yml
  - openapi/cloudhealth-reports-api-openapi.yml
  - openapi/cloudhealth-search-api-openapi.yml
  - openapi/cloudhealth-sso-api-openapi.yml
  surface: REST API (https://chapi.cloudhealthtech.com)
  type: http
- description: The same API key may instead be passed as the api_key query parameter.
  evidence: https://apidocs.cloudhealthtech.com/#documentation_how-to-use-the-cloudhealth-api
  in: query
  name: apiKeyQuery
  parameter: api_key
  surface: REST API (https://chapi.cloudhealthtech.com)
  type: apiKey
- description: 'Exchange the API key for a token pair with the loginAPI(apiKey) mutation (no auth required), then send "Authorization: Bearer <accessToken>". Access tokens are valid for 15 minutes; the refresh token (refresh(token) mutation) is valid for 9 hours. loginCspService / loginCspUser exchange VMware Cloud Services Platform tokens. FlexOrg sub-organizations require their own token.'
  evidence:
  - https://help.cloudhealthtech.com/graphql-api/#authentication
  - graphql/cloudhealth-graphql-public-schema.graphql
  name: graphqlAccessToken
  scheme: bearer
  surface: GraphQL API (https://apps.cloudhealthtech.com/graphql)
  token_exchange_operations:
  - loginAPI
  - login
  - refresh
  - loginCspService
  - loginCspUser
  token_lifetimes:
    access_token: 15 minutes
    refresh_token: 9 hours
  type: http
- authorizationUrl: https://apps.cloudhealthtech.com/oauth2/authorize
  description: 'The MCP endpoint answers unauthenticated requests with 401 and WWW-Authenticate: Bearer resource_metadata="https://apps.cloudhealthtech.com/.well-known/oauth-protected-resource" (RFC 9728). The authorization server publishes RFC 8414 metadata with PKCE (S256), dynamic client registration and client ID metadata documents.'
  evidence:
  - well-known/cloudhealth-oauth-authorization-server.json
  - well-known/cloudhealth-oauth-protected-resource.json
  flows:
  - authorizationCode
  - clientCredentials
  - refreshToken
  issuer: https://apps.cloudhealthtech.com
  jwks_uri: https://apps.cloudhealthtech.com/oauth2/jwks
  name: mcpOAuth
  pkce:
  - S256
  registrationUrl: https://apps.cloudhealthtech.com/oauth2/register
  revocationUrl: https://apps.cloudhealthtech.com/oauth2/revoke
  scope_count: 4
  scopes_ref: scopes/cloudhealth-scopes.yml
  surface: MCP server (https://apps.cloudhealthtech.com/mcp)
  tokenUrl: https://apps.cloudhealthtech.com/oauth2/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
slug: cloudhealth-authentication
source_filename: cloudhealth-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: searched\nsource: https://apidocs.cloudhealthtech.com/#documentation_getting-your-api-key\ndocs:\n  - https://apidocs.cloudhealthtech.com/#documentation_how-to-use-the-cloudhealth-api\n  - https://apidocs.cloudhealthtech.com/#documentation_getting-your-api-key\n  - https://help.cloudhealthtech.com/graphql-api/#authentication\n  - https://apps.cloudhealthtech.com/.well-known/oauth-authorization-server\nnote: Upgraded from the spec-derived profile (openapi/ files are API Evangelist-authored from the docs, see\n  openapi/_ae-authored/README.md). The REST, GraphQL and MCP surfaces authenticate three different ways.\nsummary:\n  types:\n    - http\n    - apiKey\n    - oauth2\n  api_key_in:\n    - header\n    - query\n  oauth2_flows:\n    - authorizationCode\n    - clientCredentials\n    - refreshToken\nschemes:\n  - name: bearerAuth\n    surface: REST API (https://chapi.cloudhealthtech.com)\n    type: http\n    scheme: bearer\n    description: >-\n\
  \      Per-user API key (a GUID generated under My Profile > API Key) sent as\n      \"Authorization: Bearer <api_key>\". Every request must also send Accept: application/json\n      (or Content-Type: application/json). Generating a new key invalidates the previous one; the\n      docs recommend periodic rotation. The API enforces the same organization scoping and role\n      restrictions as the CloudHealth UI.\n    evidence: https://apidocs.cloudhealthtech.com/#documentation_how-to-use-the-cloudhealth-api\n    sources:\n      - openapi/cloudhealth-aws-accounts-api-openapi.yml\n      - openapi/cloudhealth-perspectives-api-openapi.yml\n      - openapi/cloudhealth-reports-api-openapi.yml\n      - openapi/cloudhealth-search-api-openapi.yml\n      - openapi/cloudhealth-sso-api-openapi.yml\n  - name: apiKeyQuery\n    surface: REST API (https://chapi.cloudhealthtech.com)\n    type: apiKey\n    in: query\n    parameter: api_key\n    description: The same API key may instead be passed as the api_key\
  \ query parameter.\n    evidence: https://apidocs.cloudhealthtech.com/#documentation_how-to-use-the-cloudhealth-api\n  - name: graphqlAccessToken\n    surface: GraphQL API (https://apps.cloudhealthtech.com/graphql)\n    type: http\n    scheme: bearer\n    description: >-\n      Exchange the API key for a token pair with the loginAPI(apiKey) mutation (no auth required),\n      then send \"Authorization: Bearer <accessToken>\". Access tokens are valid for 15 minutes; the\n      refresh token (refresh(token) mutation) is valid for 9 hours. loginCspService / loginCspUser\n      exchange VMware Cloud Services Platform tokens. FlexOrg sub-organizations require their own\n      token.\n    token_lifetimes:\n      access_token: 15 minutes\n      refresh_token: 9 hours\n    token_exchange_operations: [loginAPI, login, refresh, loginCspService, loginCspUser]\n    evidence:\n      - https://help.cloudhealthtech.com/graphql-api/#authentication\n      - graphql/cloudhealth-graphql-public-schema.graphql\n\
  \  - name: mcpOAuth\n    surface: MCP server (https://apps.cloudhealthtech.com/mcp)\n    type: oauth2\n    description: >-\n      The MCP endpoint answers unauthenticated requests with 401 and\n      WWW-Authenticate: Bearer resource_metadata=\"https://apps.cloudhealthtech.com/.well-known/oauth-protected-resource\"\n      (RFC 9728). The authorization server publishes RFC 8414 metadata with PKCE (S256), dynamic\n      client registration and client ID metadata documents.\n    issuer: https://apps.cloudhealthtech.com\n    authorizationUrl: https://apps.cloudhealthtech.com/oauth2/authorize\n    tokenUrl: https://apps.cloudhealthtech.com/oauth2/token\n    revocationUrl: https://apps.cloudhealthtech.com/oauth2/revoke\n    registrationUrl: https://apps.cloudhealthtech.com/oauth2/register\n    jwks_uri: https://apps.cloudhealthtech.com/oauth2/jwks\n    flows: [authorizationCode, clientCredentials, refreshToken]\n    pkce: [S256]\n    token_endpoint_auth_methods: [client_secret_basic, client_secret_post,\
  \ none]\n    scope_count: 4\n    scopes_ref: scopes/cloudhealth-scopes.yml\n    evidence:\n      - well-known/cloudhealth-oauth-authorization-server.json\n      - well-known/cloudhealth-oauth-protected-resource.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudhealth/refs/heads/main/authentication/cloudhealth-authentication.yml
summary_line: http/apiKey/oauth2 · 4 schemes
tags:
- Cloud Cost
- Cloud Governance
- Cloud Management
- Cost Optimization
- FinOps
- Multi-Cloud
---
