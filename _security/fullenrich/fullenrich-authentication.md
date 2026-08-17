---
api_key_in:
- header
api_specs:
- filename: fullenrich-contact-enrichment-api-openapi.yml
  format: yaml
  label: FullEnrich Contact Enrichment API
  slug: fullenrich-contact-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullenrich/refs/heads/main/openapi/fullenrich-contact-enrichment-api-openapi.yml
- filename: fullenrich-reverse-email-lookup-api-openapi.yml
  format: yaml
  label: FullEnrich Reverse Email Lookup API
  slug: fullenrich-reverse-email-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullenrich/refs/heads/main/openapi/fullenrich-reverse-email-lookup-api-openapi.yml
- filename: fullenrich-search-api-openapi.yml
  format: yaml
  label: FullEnrich Search API
  slug: fullenrich-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullenrich/refs/heads/main/openapi/fullenrich-search-api-openapi.yml
- filename: fullenrich-lookup-api-openapi.yml
  format: yaml
  label: FullEnrich Lookup API
  slug: fullenrich-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullenrich/refs/heads/main/openapi/fullenrich-lookup-api-openapi.yml
- filename: fullenrich-account-api-openapi.yml
  format: yaml
  label: FullEnrich Account API
  slug: fullenrich-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullenrich/refs/heads/main/openapi/fullenrich-account-api-openapi.yml
auth_types:
- http
- oauth2
description: FullEnrich runs three distinct authentication surfaces. The public REST API uses a static workspace API key passed as a Bearer token. The application host runs a full OAuth 2.0 / OIDC authorization server with 13 granular scopes (discovered via RFC 8414 metadata, used by first-party integrations and Enterprise BYOK). The MCP server runs a separate authorization server with a single `api:mcp` scope and browser-based user consent. Only the first is described by the OpenAPI.
kind: authentication
layout: security
method: searched
name: Fullenrich Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: FullEnrich secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: FullEnrich
provider_slug: fullenrich
scheme_count: 3
schemes:
- applies_to: all REST operations
  bearerFormat: string
  description: 'Workspace API key from the FullEnrich dashboard, sent as `Authorization: Bearer <API_KEY>`. Applies to every REST operation. A missing or invalid key returns 401 with an `Error` body. Keys can be regenerated from the dashboard if compromised.'
  doubles_as:
    detail: The same API key is the HMAC-SHA1 secret used to sign outbound webhooks (X-Signature-SHA1). See asyncapi/fullenrich-webhooks.yml. Rotating the API key therefore also rotates webhook verification.
    purpose: webhook signing secret
  key_source: https://app.fullenrich.com/app/api
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/_original/fullenrich-openapi.yml
  type: http
- description: OAuth 2.0 authorization server on the application host. Discovered from published RFC 8414 / OIDC metadata; not referenced by the public OpenAPI, so it is not currently a documented path for third-party REST integration.
  detail: scopes/fullenrich-scopes.yml
  discovery:
  - well-known/fullenrich-app-openid-configuration.json
  - well-known/fullenrich-app-oauth-authorization-server.json
  endpoints:
    introspection: https://app.fullenrich.com/oauth2/introspect
    jwks_uri: https://app.fullenrich.com/oauth2/jwks
    revocation: https://app.fullenrich.com/oauth2/revoke
  flows:
  - authorizationUrl: https://app.fullenrich.com/oauth2/authorize
    flow: authorizationCode
    pkce:
    - S256
    tokenUrl: https://app.fullenrich.com/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://app.fullenrich.com/oauth2/token
  - flow: refreshToken
    tokenUrl: https://app.fullenrich.com/oauth2/token
  id_token_signing_alg:
  - HS256
  issuer: fullenrich
  name: FullEnrichOAuth
  scope_count: 13
  sources:
  - https://app.fullenrich.com/.well-known/openid-configuration
  token_endpoint_auth_methods:
  - none
  - client_secret_basic
  - client_secret_post
  type: oauth2
- bearer_methods_supported:
  - header
  description: Separate authorization server protecting the remote MCP server. Uses dynamic client registration and browser-based user consent — there is no static client secret for an end user to copy into an MCP client.
  discovery:
  - well-known/fullenrich-mcp-oauth-authorization-server.json
  - well-known/fullenrich-mcp-oauth-protected-resource.json
  dynamic_client_registration: true
  endpoints:
    registration: https://mcp.fullenrich.com/register
    revocation: https://mcp.fullenrich.com/revoke
  flows:
  - authorizationUrl: https://mcp.fullenrich.com/authorize
    flow: authorizationCode
    pkce:
    - S256
    tokenUrl: https://mcp.fullenrich.com/token
  - flow: refreshToken
    tokenUrl: https://mcp.fullenrich.com/token
  issuer: https://mcp.fullenrich.com
  name: FullEnrichMCPOAuth
  protected_resource: https://mcp.fullenrich.com/mcp
  scopes:
  - api:mcp
  sources:
  - https://mcp.fullenrich.com/.well-known/oauth-authorization-server
  - https://mcp.fullenrich.com/.well-known/oauth-protected-resource
  type: oauth2
slug: fullenrich-authentication
source_filename: fullenrich-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: openapi/_original/fullenrich-openapi.yml\ndocs: https://docs.fullenrich.com/api/v2/general/authentication\ndescription: >-\n  FullEnrich runs three distinct authentication surfaces. The public REST API uses\n  a static workspace API key passed as a Bearer token. The application host runs a\n  full OAuth 2.0 / OIDC authorization server with 13 granular scopes (discovered\n  via RFC 8414 metadata, used by first-party integrations and Enterprise BYOK).\n  The MCP server runs a separate authorization server with a single `api:mcp`\n  scope and browser-based user consent. Only the first is described by the OpenAPI.\n\nsummary:\n  types: [http, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken]\n  mfa_supported_for_console: unknown\n\nschemes:\n  - name: BearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: string\n    description: >-\n      Workspace API key from the\
  \ FullEnrich dashboard, sent as\n      `Authorization: Bearer <API_KEY>`. Applies to every REST operation. A missing\n      or invalid key returns 401 with an `Error` body. Keys can be regenerated from\n      the dashboard if compromised.\n    key_source: https://app.fullenrich.com/app/api\n    applies_to: all REST operations\n    sources:\n      - openapi/_original/fullenrich-openapi.yml\n    doubles_as:\n      purpose: webhook signing secret\n      detail: >-\n        The same API key is the HMAC-SHA1 secret used to sign outbound webhooks\n        (X-Signature-SHA1). See asyncapi/fullenrich-webhooks.yml. Rotating the API\n        key therefore also rotates webhook verification.\n\n  - name: FullEnrichOAuth\n    type: oauth2\n    description: >-\n      OAuth 2.0 authorization server on the application host. Discovered from\n      published RFC 8414 / OIDC metadata; not referenced by the public OpenAPI, so\n      it is not currently a documented path for third-party REST integration.\n\
  \    issuer: fullenrich\n    discovery:\n      - well-known/fullenrich-app-openid-configuration.json\n      - well-known/fullenrich-app-oauth-authorization-server.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://app.fullenrich.com/oauth2/authorize\n        tokenUrl: https://app.fullenrich.com/oauth2/token\n        pkce: [S256]\n      - flow: clientCredentials\n        tokenUrl: https://app.fullenrich.com/oauth2/token\n      - flow: refreshToken\n        tokenUrl: https://app.fullenrich.com/oauth2/token\n    endpoints:\n      jwks_uri: https://app.fullenrich.com/oauth2/jwks\n      introspection: https://app.fullenrich.com/oauth2/introspect\n      revocation: https://app.fullenrich.com/oauth2/revoke\n    token_endpoint_auth_methods: [none, client_secret_basic, client_secret_post]\n    id_token_signing_alg: [HS256]\n    scope_count: 13\n    detail: scopes/fullenrich-scopes.yml\n    sources:\n      - https://app.fullenrich.com/.well-known/openid-configuration\n\
  \n  - name: FullEnrichMCPOAuth\n    type: oauth2\n    description: >-\n      Separate authorization server protecting the remote MCP server. Uses dynamic\n      client registration and browser-based user consent — there is no static\n      client secret for an end user to copy into an MCP client.\n    issuer: https://mcp.fullenrich.com\n    discovery:\n      - well-known/fullenrich-mcp-oauth-authorization-server.json\n      - well-known/fullenrich-mcp-oauth-protected-resource.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://mcp.fullenrich.com/authorize\n        tokenUrl: https://mcp.fullenrich.com/token\n        pkce: [S256]\n      - flow: refreshToken\n        tokenUrl: https://mcp.fullenrich.com/token\n    endpoints:\n      registration: https://mcp.fullenrich.com/register\n      revocation: https://mcp.fullenrich.com/revoke\n    dynamic_client_registration: true\n    protected_resource: https://mcp.fullenrich.com/mcp\n    scopes: [api:mcp]\n    bearer_methods_supported:\
  \ [header]\n    sources:\n      - https://mcp.fullenrich.com/.well-known/oauth-authorization-server\n      - https://mcp.fullenrich.com/.well-known/oauth-protected-resource\n\nenterprise:\n  sso: Custom SSO / custom IdP available as an Enterprise add-on.\n  byok: Bring Your Own API Key (BYOK) offered on Enterprise plans.\n  google_sso: Available on every plan including the free trial.\n  source: https://fullenrich.com/pricing.md\n\nfailure_modes:\n  - status: 401\n    meaning: Missing Authorization header, or an invalid/revoked API key.\n    body: '{ \"code\": \"...\", \"message\": \"...\" }'\n\nx-evidence:\n  - url: https://docs.fullenrich.com/api/v2/general/authentication.md\n    http_status: 200\n  - url: https://app.fullenrich.com/.well-known/openid-configuration\n    http_status: 200\n  - url: https://mcp.fullenrich.com/.well-known/oauth-authorization-server\n    http_status: 200\n  - url: https://mcp.fullenrich.com/mcp\n    http_status: 401\n    detail: WWW-Authenticate Bearer resource_metadata\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fullenrich/refs/heads/main/authentication/fullenrich-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- B2B Data
- Contact Enrichment
- Email Finder
- Phone Finder
- Waterfall Enrichment
- Sales Intelligence
- People Search
- Company Search
- Reverse Email Lookup
- Agent Ready
---
