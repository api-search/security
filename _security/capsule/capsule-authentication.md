---
anonymous_access: false
api_key_in: []
api_specs:
- filename: capsule-opportunities-api-openapi.yml
  format: yaml
  label: Capsule Opportunities API
  slug: capsule-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capsule/refs/heads/main/openapi/capsule-opportunities-api-openapi.yml
- filename: capsule-parties-api-openapi.yml
  format: yaml
  label: Capsule Parties API
  slug: capsule-parties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capsule/refs/heads/main/openapi/capsule-parties-api-openapi.yml
- filename: capsule-projects-api-openapi.yml
  format: yaml
  label: Capsule Projects API
  slug: capsule-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capsule/refs/heads/main/openapi/capsule-projects-api-openapi.yml
- filename: capsule-tasks-api-openapi.yml
  format: yaml
  label: Capsule Tasks API
  slug: capsule-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capsule/refs/heads/main/openapi/capsule-tasks-api-openapi.yml
auth_types:
- http
- oauth2
- openIdConnect
description: 'Capsule authenticates every v2 REST request with a Bearer token in the Authorization header. Two token kinds exist: a personal access token minted inside a Capsule account, and an OAuth 2.0 authorization-code access token for multi-tenant applications. Upgraded from the 2026-07-11 derived profile, which recorded only the generic bearerAuth scheme from the OpenAPI.'
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Capsule Authentication
name_suffix: Authentication
oauth_flows: []
overview: Capsule secures its APIs with http, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Capsule
provider_slug: capsule
scheme_count: 3
schemes:
- description: Personal access token, generated at My Preferences > API Authentication Tokens inside a Capsule account. Suited to one-off integrations and testing. A token can be minted read-only ("Read information from your Capsule account"), which is what the Capsule MCP server asks for.
  format: 'Authorization: Bearer {token}'
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - https://developer.capsulecrm.com/v2/overview/authentication
  type: http
- access_token_ttl_note: ~7 days, stated verbatim in the docs.
  access_token_ttl_seconds: 604799
  authorizationUrl: https://api.capsulecrm.com/oauth/authorise
  flow: authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  name: oauth2
  pkce: true
  pkce_methods:
  - plain
  - S256
  refresh_token_rotation: '"Refresh tokens may be rotated; always store the most recent version."'
  refresh_tokens: true
  revocationUrl: https://api.capsulecrm.com/oauth/revoke
  revocation_note: The discovery document gives revocation_endpoint as https://api.capsulecrm.com/oauth/revoke; the authentication docs page writes it as .../oauth/token/revoke. Both are Capsule's own published values and they disagree - recorded as found, not reconciled.
  scopes:
    see: scopes/capsule-scopes.yml
  sources:
  - https://developer.capsulecrm.com/v2/overview/authentication
  - https://api.capsulecrm.com/.well-known/oauth-authorization-server
  tokenUrl: https://api.capsulecrm.com/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: oauth2
- claims_supported:
  - name
  - email
  - tenant
  - family_name
  - locale
  - iat
  - sub
  - updated_at
  - given_name
  - iss
  - exp
  - subdomain
  description: 'Capsule is a full OpenID Provider: the openid-configuration document is served, a JWKS is published, and openid/profile/email are among the supported scopes. This is not documented on the authentication docs page - it was found by probing /.well-known/ on the API host.'
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://api.capsulecrm.com
  name: openIdConnect
  openIdConnectUrl: https://api.capsulecrm.com/.well-known/openid-configuration
  sources:
  - https://api.capsulecrm.com/.well-known/openid-configuration
  type: openIdConnect
  userinfo_endpoint: https://api.capsulecrm.com/oauth/userinfo
slug: capsule-authentication
source_filename: capsule-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: https://developer.capsulecrm.com/v2/overview/authentication\ndocs: https://developer.capsulecrm.com/v2/overview/authentication\ndiscovery:\n  openid_configuration: https://api.capsulecrm.com/.well-known/openid-configuration\n  oauth_authorization_server: https://api.capsulecrm.com/.well-known/oauth-authorization-server\n  jwks_uri: https://api.capsulecrm.com/.well-known/jwks.json\n  status: 200\n  probed: '2026-09-05'\n  saved: well-known/\ndescription: >-\n  Capsule authenticates every v2 REST request with a Bearer token in the\n  Authorization header. Two token kinds exist: a personal access token minted\n  inside a Capsule account, and an OAuth 2.0 authorization-code access token\n  for multi-tenant applications. Upgraded from the 2026-07-11 derived profile,\n  which recorded only the generic bearerAuth scheme from the OpenAPI.\nsummary:\n  types:\n  - http\n  - oauth2\n  - openIdConnect\nschemes:\n- name: bearerAuth\n \
  \ type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer {token}'\n  description: >-\n    Personal access token, generated at My Preferences > API Authentication\n    Tokens inside a Capsule account. Suited to one-off integrations and\n    testing. A token can be minted read-only (\"Read information from your\n    Capsule account\"), which is what the Capsule MCP server asks for.\n  sources:\n  - https://developer.capsulecrm.com/v2/overview/authentication\n- name: oauth2\n  type: oauth2\n  flow: authorizationCode\n  pkce: true\n  pkce_methods:\n  - plain\n  - S256\n  authorizationUrl: https://api.capsulecrm.com/oauth/authorise\n  tokenUrl: https://api.capsulecrm.com/oauth/token\n  revocationUrl: https://api.capsulecrm.com/oauth/revoke\n  revocation_note: >-\n    The discovery document gives revocation_endpoint as\n    https://api.capsulecrm.com/oauth/revoke; the authentication docs page\n    writes it as .../oauth/token/revoke. Both are Capsule's\
  \ own published\n    values and they disagree - recorded as found, not reconciled.\n  grant_types:\n  - authorization_code\n  - refresh_token\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  scopes:\n    see: scopes/capsule-scopes.yml\n  access_token_ttl_seconds: 604799\n  access_token_ttl_note: ~7 days, stated verbatim in the docs.\n  refresh_tokens: true\n  refresh_token_rotation: >-\n    \"Refresh tokens may be rotated; always store the most recent version.\"\n  sources:\n  - https://developer.capsulecrm.com/v2/overview/authentication\n  - https://api.capsulecrm.com/.well-known/oauth-authorization-server\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://api.capsulecrm.com/.well-known/openid-configuration\n  issuer: https://api.capsulecrm.com\n  userinfo_endpoint: https://api.capsulecrm.com/oauth/userinfo\n  id_token_signing_alg_values_supported:\n  - RS256\n  claims_supported:\n  - name\n  - email\n  - tenant\n  - family_name\n\
  \  - locale\n  - iat\n  - sub\n  - updated_at\n  - given_name\n  - iss\n  - exp\n  - subdomain\n  description: >-\n    Capsule is a full OpenID Provider: the openid-configuration document is\n    served, a JWKS is published, and openid/profile/email are among the\n    supported scopes. This is not documented on the authentication docs page\n    - it was found by probing /.well-known/ on the API host.\n  sources:\n  - https://api.capsulecrm.com/.well-known/openid-configuration\nerrors:\n- {status: 401, meaning: invalid or expired token, header: WWW-Authenticate}\n- {status: 403, meaning: valid token without the required scope, header: WWW-Authenticate}\nmtls: false\napi_key_query_param: false\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capsule/refs/heads/main/authentication/capsule-authentication.yml
summary_line: http/oauth2/openIdConnect · 3 schemes
tags:
- Contact Management
- CRM
- Custom Fields
- Opportunities
- Pipelines
- Project Management
- REST
- Sales
- Task
- Webhook
---
