---
api_key_in:
- header
auth_types:
- http
- oauth2
- openIdConnect
description: 'The Sprout Social Public API accepts two credential types on the same Authorization bearer header: a long-lived account-scoped API token generated in the Sprout web app, and a JWT access token issued by Sprout''s Okta-hosted OAuth 2.0 authorization server. There is no OpenAPI document to derive from — this profile was read from the provider''s own documentation and from the live RFC 8414 authorization server metadata saved in well-known/.'
kind: authentication
layout: security
method: searched
name: Sprout Social Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Sprout Social secures its APIs with http, oauth2, and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Sprout Social
provider_slug: sprout-social
scheme_count: 4
schemes:
- description: Account-scoped API token. Any Sprout user holding the "API Permissions" permission can generate, view and invalidate tokens from Settings > Global Features > API > API Token Management. Tokens are customer-account scoped, not user scoped.
  format: 'Authorization: Bearer <API token>'
  in: header
  issuance: Sprout web application (Settings > Global Features > API)
  name: SproutApiToken
  parameter_name: Authorization
  scheme: bearer
  source: https://api.sproutsocial.com/docs/
  type: http
- description: Machine-to-machine authentication. Clients are provisioned under OAuth Client Management in the Sprout app ("Generate configuration" > Machine-to-machine authentication), which returns a client_id and client_secret. The published example requests scope=organization_id.
  documented_request: 'POST /v1/token with Content-Type: application/x-www-form-urlencoded and client_id, client_secret, grant_type=client_credentials, scope=organization_id'
  flow: clientCredentials
  name: SproutOAuth2ClientCredentials
  source: https://api.sproutsocial.com/docs/
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  token_url: https://identity.sproutsocial.com/oauth2/84e39c75-d770-45d9-90a9-7b79e3037d2c/v1/token
  type: oauth2
- authorization_url: https://identity.sproutsocial.com/oauth2/84e39c75-d770-45d9-90a9-7b79e3037d2c/v1/authorize
  description: User-based authentication. The OAuth client configuration requires a list of allowed redirect URIs, and the integrating application requires users to log in with Sprout.
  flow: authorizationCode
  name: SproutOAuth2AuthorizationCode
  pkce_methods:
  - S256
  refresh_supported: true
  source: well-known/sprout-social-oauth-authorization-server.json
  token_url: https://identity.sproutsocial.com/oauth2/84e39c75-d770-45d9-90a9-7b79e3037d2c/v1/token
  type: oauth2
- claims:
  - sub
  - aud
  - email
  - exp
  - family_name
  - given_name
  - iat
  - iss
  - sid
  - client_id
  - oid
  - iid
  - actor
  id_token_signing_alg_values:
  - RS256
  - ES512
  issuer: https://identity.sproutsocial.com/oauth2/84e39c75-d770-45d9-90a9-7b79e3037d2c
  jwks_uri: https://identity.sproutsocial.com/oauth2/84e39c75-d770-45d9-90a9-7b79e3037d2c/v1/jwks
  name: SproutOpenIDConnect
  openid_configuration_url: https://identity.sproutsocial.com/oauth2/84e39c75-d770-45d9-90a9-7b79e3037d2c/.well-known/openid-configuration
  source: well-known/sprout-social-openid-configuration.json
  type: openIdConnect
  userinfo_endpoint: https://identity.sproutsocial.com/oauth2/84e39c75-d770-45d9-90a9-7b79e3037d2c/v1/userinfo
slug: sprout-social-authentication
source_filename: sprout-social-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://api.sproutsocial.com/docs/\ndocs: https://api.sproutsocial.com/docs/\nname: Sprout Social API authentication profile\ndescription: >-\n  The Sprout Social Public API accepts two credential types on the same\n  Authorization bearer header: a long-lived account-scoped API token generated in the\n  Sprout web app, and a JWT access token issued by Sprout's Okta-hosted OAuth 2.0\n  authorization server. There is no OpenAPI document to derive from — this profile was\n  read from the provider's own documentation and from the live RFC 8414 authorization\n  server metadata saved in well-known/.\n\nsummary:\n  types:\n  - http\n  - oauth2\n  - openIdConnect\n  http_schemes:\n  - bearer\n  bearer_format: JWT or opaque Sprout API token\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  refresh_token_supported: true\n  pkce: true\n  mtls: false\n\nschemes:\n- name: SproutApiToken\n  type:\
  \ http\n  scheme: bearer\n  in: header\n  parameter_name: Authorization\n  format: 'Authorization: Bearer <API token>'\n  description: >-\n    Account-scoped API token. Any Sprout user holding the \"API Permissions\" permission\n    can generate, view and invalidate tokens from Settings > Global Features > API >\n    API Token Management. Tokens are customer-account scoped, not user scoped.\n  issuance: Sprout web application (Settings > Global Features > API)\n  source: https://api.sproutsocial.com/docs/\n\n- name: SproutOAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://identity.sproutsocial.com/oauth2/84e39c75-d770-45d9-90a9-7b79e3037d2c/v1/token\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  description: >-\n    Machine-to-machine authentication. Clients are provisioned under OAuth Client\n    Management in the Sprout app (\"Generate configuration\" > Machine-to-machine\n    authentication), which returns a\
  \ client_id and client_secret. The published example\n    requests scope=organization_id.\n  documented_request: >-\n    POST /v1/token with Content-Type: application/x-www-form-urlencoded and\n    client_id, client_secret, grant_type=client_credentials, scope=organization_id\n  source: https://api.sproutsocial.com/docs/\n\n- name: SproutOAuth2AuthorizationCode\n  type: oauth2\n  flow: authorizationCode\n  authorization_url: https://identity.sproutsocial.com/oauth2/84e39c75-d770-45d9-90a9-7b79e3037d2c/v1/authorize\n  token_url: https://identity.sproutsocial.com/oauth2/84e39c75-d770-45d9-90a9-7b79e3037d2c/v1/token\n  refresh_supported: true\n  pkce_methods:\n  - S256\n  description: >-\n    User-based authentication. The OAuth client configuration requires a list of allowed\n    redirect URIs, and the integrating application requires users to log in with Sprout.\n  source: well-known/sprout-social-oauth-authorization-server.json\n\n- name: SproutOpenIDConnect\n  type: openIdConnect\n  issuer:\
  \ https://identity.sproutsocial.com/oauth2/84e39c75-d770-45d9-90a9-7b79e3037d2c\n  openid_configuration_url: https://identity.sproutsocial.com/oauth2/84e39c75-d770-45d9-90a9-7b79e3037d2c/.well-known/openid-configuration\n  userinfo_endpoint: https://identity.sproutsocial.com/oauth2/84e39c75-d770-45d9-90a9-7b79e3037d2c/v1/userinfo\n  jwks_uri: https://identity.sproutsocial.com/oauth2/84e39c75-d770-45d9-90a9-7b79e3037d2c/v1/jwks\n  id_token_signing_alg_values:\n  - RS256\n  - ES512\n  claims:\n  - sub\n  - aud\n  - email\n  - exp\n  - family_name\n  - given_name\n  - iat\n  - iss\n  - sid\n  - client_id\n  - oid\n  - iid\n  - actor\n  source: well-known/sprout-social-openid-configuration.json\n\nauthorization_server:\n  issuer: https://identity.sproutsocial.com/oauth2/84e39c75-d770-45d9-90a9-7b79e3037d2c\n  metadata_url: https://identity.sproutsocial.com/oauth2/84e39c75-d770-45d9-90a9-7b79e3037d2c/.well-known/oauth-authorization-server\n  grant_types_supported:\n  - authorization_code\n\
  \  - refresh_token\n  - client_credentials\n  response_types_supported:\n  - code\n  response_modes_supported:\n  - query\n  - form_post\n  code_challenge_methods_supported:\n  - S256\n  introspection_endpoint: https://identity.sproutsocial.com/oauth2/84e39c75-d770-45d9-90a9-7b79e3037d2c/v1/introspect\n  revocation_endpoint: https://identity.sproutsocial.com/oauth2/84e39c75-d770-45d9-90a9-7b79e3037d2c/v1/revoke\n  file: well-known/sprout-social-oauth-authorization-server.json\n\naccess_requirements:\n  plan: Advanced or higher (or Enterprise)\n  plan_source: https://sproutsocial.com/pricing/\n  additional_agreement: >-\n    Access to X (Twitter) data through the Sprout API additionally requires a Sprout\n    user with the API Permissions permission to accept the Sprout API X Content End\n    User License Agreement, presented at the top of the API page under Global Features\n    in Settings.\n  terms: https://sproutsocial.com/legal/api-terms-of-service/\n\nrequest_headers:\n- header: Authorization\n\
  \  value: Bearer <OAuth access token OR API token>\n  required: true\n- header: Accept\n  value: application/json\n  required: true\n- header: Content-Type\n  value: application/json\n  required: true\n\nnotes:\n- The Authorization header accepts both account-scoped API tokens and OAuth access\n  tokens interchangeably; the API does not distinguish them at the header level.\n- No mutual TLS, no request signing, and no HTTP Basic authentication is documented\n  for the data API itself. Basic auth appears only as a token-endpoint client\n  authentication method on the authorization server.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sprout-social/refs/heads/main/authentication/sprout-social-authentication.yml
summary_line: http/oauth2/openIdConnect · 4 schemes
tags:
- Social-Media
- Social Media Management
- Publishing
- Analytics
- Reporting
- Messaging
- Listening
---
