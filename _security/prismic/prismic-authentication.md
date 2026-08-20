---
api_key_in:
- query
- header
api_specs:
- filename: TzCHBqbH
  format: yaml
  label: Prismic Types API
  slug: types-api
  spec_type: Postman
  url: https://documenter.getpostman.com/view/5743666/TzCHBqbH
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Prismic Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Prismic secures its APIs with apiKey, http, and oauth2 across 6 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Prismic
provider_slug: prismic
scheme_count: 6
schemes:
- applies_to:
  - Content API
  - Repository API
  description: A long secret string appended as a URL search parameter. Required only when the repository's API visibility is private; public ("Open API") repositories answer anonymously.
  docs: https://prismic.io/docs/content-api
  in: query
  name: contentAccessTokenQuery
  observed: Verified live — https://prismic-main.cdn.prismic.io/api/v2 and /api/v2/documents/search both returned HTTP 200 with no credential at all on 2026-08-13, because Prismic's own repository is publicly readable.
  parameter: access_token
  required: only for private repositories
  type: apiKey
- applies_to:
  - GraphQL API
  description: 'Authorization: Bearer <access-token> for private repositories querying the GraphQL endpoint.'
  docs: https://prismic.io/docs/graphql-technical-reference
  name: contentAccessTokenHeader
  required: only for private repositories
  scheme: bearer
  type: http
- applies_to:
  - Types API
  - Asset API
  - Migration API
  bearer_format: JWT
  description: A permanent bearer write token. Minted with `npx prismic token create --write`, or in the dashboard under Settings > API & Security > Write APIs. Multiple tokens can be issued for different applications. Prismic's docs warn explicitly that these tokens "carry many privileges" and must not be committed or exposed client-side.
  docs: https://prismic.io/docs/custom-types-api#authentication
  name: writeToken
  paired_header:
    description: The repository ID (e.g. `your-repo-name`). The write APIs live on shared hosts, so the target repository is named in a header rather than in the hostname.
    name: repository
    required: true
  required: always
  scheme: bearer
  transport: HTTPS only — "Calls made over plain HTTP and without authentication will fail."
  type: http
- applies_to:
  - Content API (temporary access tokens)
  description: Each repository advertises its own OAuth endpoints in the Repository API root document, for issuing temporary content access tokens.
  docs: https://prismic.io/docs/fetch-content#content-visiblity
  endpoint_pattern:
    authorizationUrl: https://{repo}.prismic.io/auth
    tokenUrl: https://{repo}.prismic.io/auth/token
  endpoints_are_per_repository: true
  flow: authorizationCode
  name: repositoryOAuth
  observed: Live Repository API response for prismic-main returned oauth_initiate=https://prismic-main.prismic.io/auth and oauth_token=https://prismic-main.prismic.io/auth/token (HTTP 200, 2026-08-13).
  scopes: []
  scopes_note: No scope vocabulary is published for this flow.
  type: oauth2
- applies_to:
  - MCP server
  authorizationUrl: https://mcp.prismic.io/authorize
  discovery:
    authorization_server: https://mcp.prismic.io/.well-known/oauth-authorization-server
    files:
    - well-known/prismic-mcp-oauth-protected-resource.json
    - well-known/prismic-mcp-oauth-authorization-server.json
    http_status: 200
    probed: '2026-08-13'
    protected_resource: https://mcp.prismic.io/.well-known/oauth-protected-resource
  docs: https://prismic.io/docs/mcp#authentication
  dynamic_client_registration: true
  flow: authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  identity_provider: prismic-auth.eu.auth0.com
  issuer: https://mcp.prismic.io/
  name: mcpOAuth
  pkce: S256
  registrationUrl: https://mcp.prismic.io/register
  revocationUrl: https://mcp.prismic.io/revoke
  scopes: []
  scopes_note: '`scopes_supported` is absent from the authorization-server metadata. Authorization is not scope-based: the MCP server acts as the signed-in Prismic user, so reach is bounded by that account''s repository access and role. `publish_release` additionally requires a Publisher (Manager) role. Because there is no published scope vocabulary, no scopes/ artifact is emitted.'
  tokenUrl: https://mcp.prismic.io/token
  token_endpoint_auth_methods:
  - client_secret_post
  - none
  type: oauth2
- applies_to:
  - Prismic CLI
  description: '`npx prismic login` opens a browser sign-in; `npx prismic whoami` reports the logged-in account; `npx prismic logout` clears it.'
  docs: https://prismic.io/docs/cli
  flow: authorizationCode
  name: cliSession
  type: oauth2
slug: prismic-authentication
source_filename: prismic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://prismic.io/docs/custom-types-api\ndocs:\n  - https://prismic.io/docs/custom-types-api#authentication\n  - https://prismic.io/docs/fetch-content#content-visiblity\n  - https://prismic.io/docs/mcp#authentication\n  - https://prismic.io/docs/cli\nnote: >-\n  Derived-from-OpenAPI was not possible: Prismic publishes no OpenAPI for any of\n  its seven HTTP APIs (`derive-authentication.py prismic` produced no profile).\n  Everything below was read from Prismic's own documentation, and the two OAuth\n  discovery documents were fetched live from mcp.prismic.io.\nsummary:\n  types: [apiKey, http, oauth2]\n  api_key_in: [query, header]\n  oauth2_flows: [authorizationCode]\n  read_write_split: true\n  read_write_note: >-\n    Prismic splits credentials by direction. READ (Content / Repository / Tags /\n    GraphQL) uses an access token, and is optional entirely — a repository set to\n    \"Open API\" visibility needs no credential\
  \ at all. WRITE (Types / Asset /\n    Migration) requires a bearer WRITE token, which is a different artifact minted\n    a different way. The MCP server uses neither: it is OAuth against the user's\n    own Prismic identity.\nschemes:\n  - name: contentAccessTokenQuery\n    type: apiKey\n    in: query\n    parameter: access_token\n    applies_to: [Content API, Repository API]\n    required: only for private repositories\n    docs: https://prismic.io/docs/content-api\n    description: >-\n      A long secret string appended as a URL search parameter. Required only when\n      the repository's API visibility is private; public (\"Open API\") repositories\n      answer anonymously.\n    observed: >-\n      Verified live — https://prismic-main.cdn.prismic.io/api/v2 and\n      /api/v2/documents/search both returned HTTP 200 with no credential at all\n      on 2026-08-13, because Prismic's own repository is publicly readable.\n  - name: contentAccessTokenHeader\n    type: http\n    scheme:\
  \ bearer\n    applies_to: [GraphQL API]\n    required: only for private repositories\n    docs: https://prismic.io/docs/graphql-technical-reference\n    description: 'Authorization: Bearer <access-token> for private repositories querying\n      the GraphQL endpoint.'\n  - name: writeToken\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    applies_to: [Types API, Asset API, Migration API]\n    required: always\n    docs: https://prismic.io/docs/custom-types-api#authentication\n    description: >-\n      A permanent bearer write token. Minted with `npx prismic token create\n      --write`, or in the dashboard under Settings > API & Security > Write APIs.\n      Multiple tokens can be issued for different applications. Prismic's docs\n      warn explicitly that these tokens \"carry many privileges\" and must not be\n      committed or exposed client-side.\n    paired_header:\n      name: repository\n      required: true\n      description: The repository ID (e.g. `your-repo-name`).\
  \ The write APIs live on\n        shared hosts, so the target repository is named in a header rather than in\n        the hostname.\n    transport: HTTPS only — \"Calls made over plain HTTP and without authentication\n      will fail.\"\n  - name: repositoryOAuth\n    type: oauth2\n    flow: authorizationCode\n    applies_to: [Content API (temporary access tokens)]\n    docs: https://prismic.io/docs/fetch-content#content-visiblity\n    description: >-\n      Each repository advertises its own OAuth endpoints in the Repository API\n      root document, for issuing temporary content access tokens.\n    endpoints_are_per_repository: true\n    endpoint_pattern:\n      authorizationUrl: https://{repo}.prismic.io/auth\n      tokenUrl: https://{repo}.prismic.io/auth/token\n    observed: >-\n      Live Repository API response for prismic-main returned\n      oauth_initiate=https://prismic-main.prismic.io/auth and\n      oauth_token=https://prismic-main.prismic.io/auth/token (HTTP 200, 2026-08-13).\n\
  \    scopes: []\n    scopes_note: No scope vocabulary is published for this flow.\n  - name: mcpOAuth\n    type: oauth2\n    flow: authorizationCode\n    pkce: S256\n    applies_to: [MCP server]\n    docs: https://prismic.io/docs/mcp#authentication\n    discovery:\n      protected_resource: https://mcp.prismic.io/.well-known/oauth-protected-resource\n      authorization_server: https://mcp.prismic.io/.well-known/oauth-authorization-server\n      probed: '2026-08-13'\n      http_status: 200\n      files:\n        - well-known/prismic-mcp-oauth-protected-resource.json\n        - well-known/prismic-mcp-oauth-authorization-server.json\n    issuer: https://mcp.prismic.io/\n    authorizationUrl: https://mcp.prismic.io/authorize\n    tokenUrl: https://mcp.prismic.io/token\n    revocationUrl: https://mcp.prismic.io/revoke\n    registrationUrl: https://mcp.prismic.io/register\n    dynamic_client_registration: true\n    grant_types: [authorization_code, refresh_token]\n    token_endpoint_auth_methods:\
  \ [client_secret_post, none]\n    scopes: []\n    scopes_note: >-\n      `scopes_supported` is absent from the authorization-server metadata.\n      Authorization is not scope-based: the MCP server acts as the signed-in\n      Prismic user, so reach is bounded by that account's repository access and\n      role. `publish_release` additionally requires a Publisher (Manager) role.\n      Because there is no published scope vocabulary, no scopes/ artifact is\n      emitted.\n    identity_provider: prismic-auth.eu.auth0.com\n  - name: cliSession\n    type: oauth2\n    flow: authorizationCode\n    applies_to: [Prismic CLI]\n    docs: https://prismic.io/docs/cli\n    description: '`npx prismic login` opens a browser sign-in; `npx prismic whoami`\n      reports the logged-in account; `npx prismic logout` clears it.'\nidentity_platform:\n  provider: Auth0 (EU tenant)\n  host: prismic-auth.eu.auth0.com\n  evidence: >-\n    Prismic's MCP troubleshooting instructions tell users to reset a stuck session\n\
  \    at https://prismic-auth.eu.auth0.com/v2/logout.\n  changelog: 'New authentication system, 2025-05-12 (https://prismic.io/updates/new-authentication-system)'\nsso:\n  supported: true\n  tier: Enterprise only\n  source: https://prismic.io/docs/users\ngaps:\n  - No OpenAPI or other machine-readable description of any HTTP API, so no\n    securityScheme can be parsed rather than read.\n  - No OAuth scope vocabulary on either OAuth surface.\n  - No token rotation, expiry or revocation policy published for write tokens\n    (they are described as \"permanent\").\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prismic/refs/heads/main/authentication/prismic-authentication.yml
summary_line: apiKey/http/oauth2 · 6 schemes
tags:
- GraphQL
- Headless CMS
- Content Management
- Page Builder
- JAMstack
- Marketing
- Content Delivery
- Developer Tools
- MCP
- Webhook
- Localization
- Digital Asset Management
---
