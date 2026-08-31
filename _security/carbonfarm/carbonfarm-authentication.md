---
api_key_in:
- header
- query
api_specs:
- filename: carbonfarm-assets-api-openapi.yml
  format: yaml
  label: CarbonFarm Assets API
  slug: carbonfarm-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carbonfarm/refs/heads/main/openapi/carbonfarm-assets-api-openapi.yml
- filename: carbonfarm-authentication-api-openapi.yml
  format: yaml
  label: CarbonFarm Authentication API
  slug: carbonfarm-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carbonfarm/refs/heads/main/openapi/carbonfarm-authentication-api-openapi.yml
- filename: carbonfarm-files-api-openapi.yml
  format: yaml
  label: CarbonFarm Files API
  slug: carbonfarm-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carbonfarm/refs/heads/main/openapi/carbonfarm-files-api-openapi.yml
- filename: carbonfarm-items-api-openapi.yml
  format: yaml
  label: CarbonFarm Items API
  slug: carbonfarm-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carbonfarm/refs/heads/main/openapi/carbonfarm-items-api-openapi.yml
- filename: carbonfarm-itemspost-api-openapi.yml
  format: yaml
  label: CarbonFarm Items Post API
  slug: carbonfarm-itemspost-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carbonfarm/refs/heads/main/openapi/carbonfarm-itemspost-api-openapi.yml
- filename: carbonfarm-server-api-openapi.yml
  format: yaml
  label: CarbonFarm Server API
  slug: carbonfarm-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carbonfarm/refs/heads/main/openapi/carbonfarm-server-api-openapi.yml
auth_types:
- apiKey
- openIdConnect
description: ''
kind: authentication
layout: security
method: probed
name: Carbonfarm Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
- deviceCode
overview: CarbonFarm secures its APIs with apiKey and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, refreshToken, and deviceCode flow(s).
provider_name: CarbonFarm
provider_slug: carbonfarm
scheme_count: 3
schemes:
- in: query
  name: KeyAuth
  note: Directus static access token passed as a query parameter. Directus' own guidance is to prefer the header form; a token in a query string lands in access logs and Referer headers.
  parameter: access_token
  sources:
  - openapi/carbonfarm-cms-openapi.json
  type: apiKey
- in: header
  name: Auth
  note: 'Bearer form: `Authorization: Bearer <static-or-session-token>`.'
  parameter: Authorization
  sources:
  - openapi/carbonfarm-cms-openapi.json
  type: apiKey
- dpop_signing_algs:
  - ES256
  endpoints:
    authorization: https://auth.carbonfarm.tech/authorize
    device_authorization: https://auth.carbonfarm.tech/oauth/device/code
    dynamic_registration: https://auth.carbonfarm.tech/oidc/register
    end_session: https://auth.carbonfarm.tech/oidc/logout
    jwks: https://auth.carbonfarm.tech/.well-known/jwks.json
    revocation: https://auth.carbonfarm.tech/oauth/revoke
    token: https://auth.carbonfarm.tech/oauth/token
    userinfo: https://auth.carbonfarm.tech/userinfo
  grant_types_supported:
  - authorization_code
  - client_credentials
  - refresh_token
  - implicit
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  http_status: 200
  id_token_signing_algs:
  - RS256
  - PS256
  - HS256
  issuer: https://auth.carbonfarm.tech/
  name: Auth0 OIDC (client platform)
  note: 'Organization-scoped login: app.carbonfarm.tech redirects with `organization=org_PyIwqJe0CACfELBB&organization_name=carbonfarm`, so access is bound to an Auth0 organization — a tenant must exist before a login can succeed. The scope set is Auth0''s default OIDC claim set, not an API permission model; no resource-server scopes are advertised, and /.well-known/oauth-protected-resource returns 404. That is why no `scopes/` artifact was written — there is no API scope surface to record, only OIDC identity claims.'
  openIdConnectUrl: https://auth.carbonfarm.tech/.well-known/openid-configuration
  pkce:
    code_challenge_methods:
    - S256
    - plain
    supported: true
  probed: true
  scopes_advertised:
  - openid
  - profile
  - offline_access
  - email
  - email_verified
  - name
  - given_name
  - family_name
  - nickname
  - picture
  - phone
  - address
  - created_at
  - identities
  sources:
  - well-known/carbonfarm-openid-configuration.json
  type: openIdConnect
slug: carbonfarm-authentication
source_filename: carbonfarm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: >-\n  openapi/carbonfarm-cms-openapi.json (securitySchemes) +\n  https://auth.carbonfarm.tech/.well-known/openid-configuration (live probe)\nsummary:\n  types:\n  - apiKey\n  - openIdConnect\n  api_key_in:\n  - header\n  - query\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - refreshToken\n  - deviceCode\n  note: >-\n    Two distinct authentication surfaces, and they belong to different systems. The CMS content\n    API authenticates with a Directus static token or session bearer token; the client platform\n    authenticates humans through CarbonFarm's Auth0 tenant. Neither is documented publicly —\n    everything below was read off machine-readable endpoints the company serves anonymously.\nschemes:\n- name: KeyAuth\n  type: apiKey\n  in: query\n  parameter: access_token\n  sources:\n  - openapi/carbonfarm-cms-openapi.json\n  note: >-\n    Directus static access token passed as a query parameter. Directus'\
  \ own guidance is to prefer\n    the header form; a token in a query string lands in access logs and Referer headers.\n- name: Auth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/carbonfarm-cms-openapi.json\n  note: 'Bearer form: `Authorization: Bearer <static-or-session-token>`.'\n- name: Auth0 OIDC (client platform)\n  type: openIdConnect\n  openIdConnectUrl: https://auth.carbonfarm.tech/.well-known/openid-configuration\n  issuer: https://auth.carbonfarm.tech/\n  sources:\n  - well-known/carbonfarm-openid-configuration.json\n  probed: true\n  http_status: 200\n  endpoints:\n    authorization: https://auth.carbonfarm.tech/authorize\n    token: https://auth.carbonfarm.tech/oauth/token\n    userinfo: https://auth.carbonfarm.tech/userinfo\n    jwks: https://auth.carbonfarm.tech/.well-known/jwks.json\n    revocation: https://auth.carbonfarm.tech/oauth/revoke\n    device_authorization: https://auth.carbonfarm.tech/oauth/device/code\n    end_session: https://auth.carbonfarm.tech/oidc/logout\n\
  \    dynamic_registration: https://auth.carbonfarm.tech/oidc/register\n  grant_types_supported:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - implicit\n  - password\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  scopes_advertised:\n  - openid\n  - profile\n  - offline_access\n  - email\n  - email_verified\n  - name\n  - given_name\n  - family_name\n  - nickname\n  - picture\n  - phone\n  - address\n  - created_at\n  - identities\n  pkce:\n    supported: true\n    code_challenge_methods:\n    - S256\n    - plain\n  id_token_signing_algs:\n  - RS256\n  - PS256\n  - HS256\n  dpop_signing_algs:\n  - ES256\n  note: >-\n    Organization-scoped login: app.carbonfarm.tech redirects with\n    `organization=org_PyIwqJe0CACfELBB&organization_name=carbonfarm`, so access is bound to an\n    Auth0 organization — a tenant must exist before a login can succeed. The scope\
  \ set is Auth0's\n    default OIDC claim set, not an API permission model; no resource-server scopes are advertised,\n    and /.well-known/oauth-protected-resource returns 404. That is why no `scopes/` artifact was\n    written — there is no API scope surface to record, only OIDC identity claims.\nobserved_failures:\n- request: GET https://cms.int.carbonfarm.app/items/post?limit=1\n  status: 403\n  body: '{\"errors\":[{\"message\":\"You don''t have permission to access this.\",\"extensions\":{\"code\":\"FORBIDDEN\"}}]}'\n- request: GET https://cms.int.carbonfarm.app/users/me\n  status: 401\n  body: '{\"errors\":[{\"message\":\"Invalid user credentials.\",\"extensions\":{\"code\":\"INVALID_CREDENTIALS\"}}]}'\ndocs: null\ndocs_note: >-\n  CarbonFarm publishes no authentication documentation. There is no developer portal, no API\n  reference, and no getting-started page anywhere on carbonfarm.tech — the site's only\n  developer-adjacent link is \"Client Login\".\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carbonfarm/refs/heads/main/authentication/carbonfarm-authentication.yml
summary_line: apiKey/openIdConnect · 3 schemes
tags:
- Company
- Climate Tech
- Carbon Credits
- Agriculture
- MRV
- Satellite Imagery
- Remote Sensing
- Machine-Learning
- Sustainability
- Content Management
---
