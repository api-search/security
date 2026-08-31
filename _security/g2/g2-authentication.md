---
api_key_in: []
api_specs:
- filename: g2-api-v2-openapi.yaml
  format: yaml
  label: G2 API
  slug: g2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/g2/refs/heads/main/openapi/g2-api-v2-openapi.yaml
- filename: g2-data-solutions-openapi.yaml
  format: yaml
  label: G2 Data Solutions API
  slug: g2-data-solutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/g2/refs/heads/main/openapi/g2-data-solutions-openapi.yaml
auth_types:
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: G2 Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: G2 secures its APIs with http, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: G2
provider_slug: g2
scheme_count: 3
schemes:
- expiry: One year after creation; regenerate to continue access.
  header: 'Authorization: Bearer <token>'
  issued_at: https://my.g2.com/developers
  name: AccountAPIToken
  permissions: Per-endpoint Access selection made at token creation. Endpoints left unselected are not accessible with that token, which is why a 403 here is frequently a token-configuration problem rather than a plan problem.
  resource_owner: user | organization
  revocation: Managed in the Developer Portal Access Tokens panel.
  scheme: bearer
  sources:
  - openapi/g2-api-v2-openapi.yaml
  - openapi/g2-data-solutions-openapi.yaml
  type: http
- client_registration:
    confidential_clients: supported
    dynamic: false
    manual: https://my.g2.com/developers
    note: Dynamic Client Registration (RFC 7591) is explicitly unsupported; clients must be pre-registered. The authorization callback returns `code` WITHOUT `state`, which breaks MCP SDK examples that require it.
    redirect_uri_matching: exact
  flows:
  - authorizationUrl: https://www.g2.com/oauth/authorize
    flow: authorizationCode
    introspectionUrl: https://www.g2.com/oauth/introspect
    jwksUri: https://www.g2.com/oauth/discovery/keys
    pkce: S256
    refresh_token: supported
    revocationUrl: https://www.g2.com/oauth/revoke
    scopes: see scopes/g2-scopes.yml
    tokenUrl: https://www.g2.com/oauth/token
    userinfoUrl: https://www.g2.com/oauth/userinfo
  name: G2OAuth
  sources:
  - openapi/g2-api-v2-openapi.yaml
  - openapi/g2-data-solutions-openapi.yaml
  type: oauth2
- discovery: https://www.g2.com/.well-known/openid-configuration
  file: well-known/g2-openid-configuration.json
  grant_types:
  - authorization_code
  - implicit_oidc
  - refresh_token
  id_token_alg: RS256
  issuer: https://g2.com
  name: OpenID Connect
  note: Declared as an OIDC provider through discovery rather than as an openIdConnect securityScheme in the OpenAPI; the OpenAPI models the same authorization server as oauth2 + the `openid`/`profile` scopes.
  subject_types:
  - pairwise
  token_endpoint_auth:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
slug: g2-authentication
source_filename: g2-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: >-\n  openapi/g2-api-v2-openapi.yaml, openapi/g2-data-solutions-openapi.yaml,\n  well-known/g2-openid-configuration.json,\n  https://documentation.g2.com/docs/developer-portal\ndocs: https://documentation.g2.com/docs/developer-portal\nprovider: G2\nproviderId: g2\nsummary:\n  types: [http, oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  default_posture: >-\n    Every operation in both specs is protected. Operations declare AccountAPIToken and G2OAuth\n    together, so a caller may present either a Developer Portal account token or an OAuth\n    bearer token.\nschemes:\n  - name: AccountAPIToken\n    type: http\n    scheme: bearer\n    header: 'Authorization: Bearer <token>'\n    issued_at: https://my.g2.com/developers\n    resource_owner: user | organization\n    expiry: One year after creation; regenerate to continue access.\n    permissions: >-\n      Per-endpoint Access selection made at token creation. Endpoints\
  \ left unselected are not\n      accessible with that token, which is why a 403 here is frequently a token-configuration\n      problem rather than a plan problem.\n    revocation: Managed in the Developer Portal Access Tokens panel.\n    sources: [openapi/g2-api-v2-openapi.yaml, openapi/g2-data-solutions-openapi.yaml]\n  - name: G2OAuth\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://www.g2.com/oauth/authorize\n        tokenUrl: https://www.g2.com/oauth/token\n        revocationUrl: https://www.g2.com/oauth/revoke\n        introspectionUrl: https://www.g2.com/oauth/introspect\n        userinfoUrl: https://www.g2.com/oauth/userinfo\n        jwksUri: https://www.g2.com/oauth/discovery/keys\n        pkce: S256\n        refresh_token: supported\n        scopes: see scopes/g2-scopes.yml\n    client_registration:\n      dynamic: false\n      manual: https://my.g2.com/developers\n      confidential_clients: supported\n      redirect_uri_matching:\
  \ exact\n      note: >-\n        Dynamic Client Registration (RFC 7591) is explicitly unsupported; clients must be\n        pre-registered. The authorization callback returns `code` WITHOUT `state`, which breaks\n        MCP SDK examples that require it.\n    sources: [openapi/g2-api-v2-openapi.yaml, openapi/g2-data-solutions-openapi.yaml]\n  - name: OpenID Connect\n    type: openIdConnect\n    discovery: https://www.g2.com/.well-known/openid-configuration\n    issuer: https://g2.com\n    id_token_alg: RS256\n    subject_types: [pairwise]\n    grant_types: [authorization_code, implicit_oidc, refresh_token]\n    token_endpoint_auth: [client_secret_basic, client_secret_post]\n    file: well-known/g2-openid-configuration.json\n    note: >-\n      Declared as an OIDC provider through discovery rather than as an openIdConnect\n      securityScheme in the OpenAPI; the OpenAPI models the same authorization server as\n      oauth2 + the `openid`/`profile` scopes.\nmcp_authentication:\n  endpoint:\
  \ https://mcp.g2.com/mcp\n  type: oauth2\n  flow: authorization_code_pkce\n  token_validation: >-\n    The MCP server validates access tokens against G2's introspection endpoint using its own\n    server-side credentials. Cross-application token introspection may need to be enabled on\n    the caller's OAuth app, otherwise a valid OAuth flow still yields 401 from the MCP server.\n  see_also: mcp/g2-mcp.yml\nfailure_modes:\n  - status: 401\n    title: Bad Credentials\n    causes: [missing token, malformed token, expired token (1-year account-token life), revoked token]\n  - status: 403\n    title: 'Missing <scope> scope'\n    causes: [OAuth app permission not enabled, scope not requested at authorization time]\n  - status: 403\n    title: Your current plan does not provide access to this resource\n    causes: [subscription entitlement, not authorization]\n    note: Not retryable. See errors/g2-problem-types.yml.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/g2/refs/heads/main/authentication/g2-authentication.yml
summary_line: http/oauth2/openIdConnect · 3 schemes
tags:
- B2B
- Software Discovery
- Software Reviews
- Buyer Intent
- Market Intelligence
- Product Catalog
- Competitive Intelligence
- Reviews
- Data Solutions
- MCP
---
