---
api_key_in:
- header
- query
auth_types:
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Supermetrics Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Supermetrics secures its APIs with http, oauth2, and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Supermetrics
provider_slug: supermetrics
scheme_count: 4
schemes:
- description: 'Access to the Supermetrics API is through an API key plus a valid Supermetrics API license. Preferred transport is the Authorization header "Authorization: Bearer <api key>"; an api_key query/body parameter is also accepted.'
  name: ApiKeyBearer
  scheme: bearer
  sources:
  - docs/apidocs/authentication
  type: http
- description: API key passed as the api_key request parameter (header form preferred).
  in: query
  name: ApiKeyQuery
  parameter_name: api_key
  sources:
  - docs/apidocs/authentication
  type: apiKey
- description: 'Full OAuth2 / OIDC surface advertised at api.supermetrics.com. Supports authorization_code and refresh_token grants, PKCE (S256), Dynamic Client Registration (RFC 7591), and the client_id metadata document. Token endpoint auth methods: client_secret_post, client_secret_basic, none.'
  flows:
  - authorizationUrl: https://api.supermetrics.com/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://api.supermetrics.com/oauth/token
    registrationUrl: https://api.supermetrics.com/oauth/register
    revocationUrl: https://api.supermetrics.com/oauth/revoke
    scope_count: 13
    tokenUrl: https://api.supermetrics.com/oauth/token
  name: OAuth2
  sources:
  - well-known/supermetrics-openid-configuration.json
  type: oauth2
- id_token_signing_alg:
  - RS256
  jwks_uri: https://api.supermetrics.com/oauth/certs
  name: OpenIDConnect
  openIdConnectUrl: https://api.supermetrics.com/.well-known/openid-configuration
  sources:
  - well-known/supermetrics-openid-configuration.json
  type: openIdConnect
  userinfo_endpoint: https://api.supermetrics.com/oauth/userinfo
slug: supermetrics-authentication
source_filename: supermetrics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.supermetrics.com/apidocs/authentication.md\ndocs: https://docs.supermetrics.com/apidocs/authentication\noauth_docs: https://supermetrics.com/docs/product-api-oauth/\ndiscovery:\n  openid_configuration: https://api.supermetrics.com/.well-known/openid-configuration\n  oauth_authorization_server: https://api.supermetrics.com/.well-known/oauth-authorization-server\nsummary:\n  types: [http, oauth2, openIdConnect]\n  api_key_in: [header, query]\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: ApiKeyBearer\n  type: http\n  scheme: bearer\n  description: >-\n    Access to the Supermetrics API is through an API key plus a valid Supermetrics\n    API license. Preferred transport is the Authorization header\n    \"Authorization: Bearer <api key>\"; an api_key query/body parameter is also accepted.\n  sources: [docs/apidocs/authentication]\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter_name: api_key\n\
  \  description: API key passed as the api_key request parameter (header form preferred).\n  sources: [docs/apidocs/authentication]\n- name: OAuth2\n  type: oauth2\n  description: >-\n    Full OAuth2 / OIDC surface advertised at api.supermetrics.com. Supports\n    authorization_code and refresh_token grants, PKCE (S256), Dynamic Client\n    Registration (RFC 7591), and the client_id metadata document. Token endpoint auth\n    methods: client_secret_post, client_secret_basic, none.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.supermetrics.com/oauth/authorize\n    tokenUrl: https://api.supermetrics.com/oauth/token\n    refreshUrl: https://api.supermetrics.com/oauth/token\n    registrationUrl: https://api.supermetrics.com/oauth/register\n    revocationUrl: https://api.supermetrics.com/oauth/revoke\n    scope_count: 13\n  sources: [well-known/supermetrics-openid-configuration.json]\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://api.supermetrics.com/.well-known/openid-configuration\n\
  \  id_token_signing_alg: [RS256]\n  userinfo_endpoint: https://api.supermetrics.com/oauth/userinfo\n  jwks_uri: https://api.supermetrics.com/oauth/certs\n  sources: [well-known/supermetrics-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/supermetrics/refs/heads/main/authentication/supermetrics-authentication.yml
summary_line: http/oauth2/openIdConnect · 4 schemes
tags:
- Company
- Marketing
- Analytics
- Advertising
- Data
- Reporting
- Business Intelligence
- Data Warehouse
---
