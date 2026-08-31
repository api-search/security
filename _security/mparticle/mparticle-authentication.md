---
api_key_in:
- header
api_specs:
- filename: mparticle-data-plan-api-openapi.yml
  format: yaml
  label: mParticle Data Plan API
  slug: mparticle-data-plan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mparticle/refs/heads/main/openapi/mparticle-data-plan-api-openapi.yml
- filename: mparticle-data-plan-version-api-openapi.yml
  format: yaml
  label: mParticle Data Plan Version API
  slug: mparticle-data-plan-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mparticle/refs/heads/main/openapi/mparticle-data-plan-version-api-openapi.yml
- filename: mparticle-events-api-openapi.yml
  format: yaml
  label: mParticle Events API
  slug: mparticle-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mparticle/refs/heads/main/openapi/mparticle-events-api-openapi.yml
- filename: mparticle-identify-api-openapi.yml
  format: yaml
  label: mParticle Identify API
  slug: mparticle-identify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mparticle/refs/heads/main/openapi/mparticle-identify-api-openapi.yml
- filename: mparticle-login-api-openapi.yml
  format: yaml
  label: mParticle Login API
  slug: mparticle-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mparticle/refs/heads/main/openapi/mparticle-login-api-openapi.yml
- filename: mparticle-logout-api-openapi.yml
  format: yaml
  label: mParticle Logout API
  slug: mparticle-logout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mparticle/refs/heads/main/openapi/mparticle-logout-api-openapi.yml
- filename: mparticle-modify-api-openapi.yml
  format: yaml
  label: mParticle Modify API
  slug: mparticle-modify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mparticle/refs/heads/main/openapi/mparticle-modify-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Mparticle Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: mParticle secures its APIs with apiKey, http, and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: mParticle
provider_slug: mparticle
scheme_count: 5
schemes:
- applies_to:
  - mParticle Events API
  - mParticle IDSync API
  description: HTTP Basic using the workspace server-side API key as the username and the API secret as the password. Used by the Events API (s2s.mparticle.com) and accepted by IDSync.
  name: basic
  scheme: basic
  sources:
  - openapi/mparticle-events-openapi-original.yml
  - openapi/mparticle-identity-swagger-original.yml
  - https://docs.mparticle.com/developers/apis/http/
  type: http
- description: Basic authorization with your workspace API key and secret.
  name: BasicSecurity
  scheme: basic
  sources:
  - openapi/mparticle-identity-swagger-original.yml
  type: http
- description: HMAC request digest (mParticle's recommended IDSync scheme). Requires three headers - x-mp-key (the API key), Date (ISO 8601), and x-mp-signature (hex HMAC-SHA256 of "<HTTP METHOD>\n<ISO 8601 date>\n<request path><request body>" keyed with the API secret).
  headers:
  - x-mp-key
  - x-mp-signature
  - Date
  in: header
  name: ApiKeyDigest
  parameter: x-mp-key
  sources:
  - openapi/mparticle-identity-swagger-original.yml
  - https://docs.mparticle.com/developers/apis/idsync/
  type: apiKey
- bearerFormat: JWT
  description: Bearer JWT obtained from the OAuth 2.0 client-credentials token endpoint below. Used by the Platform API, Data Planning API and Warehouse Sync API.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/mparticle-dataplanning-openapi-original.yml
  - https://docs.mparticle.com/developers/apis/platform/overview/
  type: http
- audience: https://api.mparticle.com
  description: 'OAuth 2.0 client-credentials grant. POST client_id, client_secret, audience (https://api.mparticle.com) and grant_type=client_credentials to the token endpoint; the returned access_token is sent as "Authorization: Bearer {access_token}". mParticle documents no scope parameter - authorization is carried by the credential and the AccountId/workspace_id in the request path or query string. Tokens cannot be revoked and expire in roughly 8 hours, so the docs require token caching.'
  flow: clientCredentials
  grant_type: client_credentials
  name: oauth2ClientCredentials
  revocable: false
  scopes: []
  sources:
  - https://docs.mparticle.com/developers/apis/platform/overview/
  - https://docs.mparticle.com/developers/apis/dataplanning-api/
  - well-known/mparticle-openid-configuration.json
  token_lifetime: ~8 hours
  token_url: https://sso.auth.mparticle.com/oauth/token
  type: oauth2
slug: mparticle-authentication
source_filename: mparticle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/mparticle-dataplanning-openapi-original.yml, openapi/mparticle-identity-swagger-original.yml, openapi/mparticle-events-openapi-original.yml\ndocs:\n  - https://docs.mparticle.com/developers/apis/http/\n  - https://docs.mparticle.com/developers/apis/idsync/\n  - https://docs.mparticle.com/developers/apis/platform/overview/\n  - https://docs.mparticle.com/developers/apis/dataplanning-api/\n  - https://docs.mparticle.com/developers/apis/warehouse-sync-api/overview/\nsummary:\n  types:\n    - apiKey\n    - http\n    - oauth2\n  api_key_in:\n    - header\n  oauth2_flows:\n    - clientCredentials\n  note: >-\n    mParticle splits authentication by API family. The data-ingestion APIs (Events, IDSync)\n    use workspace API key/secret credentials over HTTP Basic or an HMAC-SHA256 request digest.\n    The management APIs (Platform, Data Planning, Warehouse Sync) use OAuth 2.0 client\n    credentials against an Auth0-hosted tenant\
  \ and a bearer JWT.\nschemes:\n  - name: basic\n    type: http\n    scheme: basic\n    description: >-\n      HTTP Basic using the workspace server-side API key as the username and the API secret as\n      the password. Used by the Events API (s2s.mparticle.com) and accepted by IDSync.\n    applies_to:\n      - mParticle Events API\n      - mParticle IDSync API\n    sources:\n      - openapi/mparticle-events-openapi-original.yml\n      - openapi/mparticle-identity-swagger-original.yml\n      - https://docs.mparticle.com/developers/apis/http/\n  - name: BasicSecurity\n    type: http\n    scheme: basic\n    description: Basic authorization with your workspace API key and secret.\n    sources:\n      - openapi/mparticle-identity-swagger-original.yml\n  - name: ApiKeyDigest\n    type: apiKey\n    in: header\n    parameter: x-mp-key\n    description: >-\n      HMAC request digest (mParticle's recommended IDSync scheme). Requires three headers -\n      x-mp-key (the API key), Date (ISO 8601),\
  \ and x-mp-signature (hex HMAC-SHA256 of\n      \"<HTTP METHOD>\\n<ISO 8601 date>\\n<request path><request body>\" keyed with the API secret).\n    headers:\n      - x-mp-key\n      - x-mp-signature\n      - Date\n    sources:\n      - openapi/mparticle-identity-swagger-original.yml\n      - https://docs.mparticle.com/developers/apis/idsync/\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: >-\n      Bearer JWT obtained from the OAuth 2.0 client-credentials token endpoint below. Used by\n      the Platform API, Data Planning API and Warehouse Sync API.\n    sources:\n      - openapi/mparticle-dataplanning-openapi-original.yml\n      - https://docs.mparticle.com/developers/apis/platform/overview/\n  - name: oauth2ClientCredentials\n    type: oauth2\n    flow: clientCredentials\n    token_url: https://sso.auth.mparticle.com/oauth/token\n    audience: https://api.mparticle.com\n    grant_type: client_credentials\n    token_lifetime: ~8 hours\n\
  \    revocable: false\n    scopes: []\n    description: >-\n      OAuth 2.0 client-credentials grant. POST client_id, client_secret, audience\n      (https://api.mparticle.com) and grant_type=client_credentials to the token endpoint; the\n      returned access_token is sent as \"Authorization: Bearer {access_token}\". mParticle\n      documents no scope parameter - authorization is carried by the credential and the\n      AccountId/workspace_id in the request path or query string. Tokens cannot be revoked and\n      expire in roughly 8 hours, so the docs require token caching.\n    sources:\n      - https://docs.mparticle.com/developers/apis/platform/overview/\n      - https://docs.mparticle.com/developers/apis/dataplanning-api/\n      - well-known/mparticle-openid-configuration.json\ndiscovery:\n  openid_configuration: well-known/mparticle-openid-configuration.json\n  issuer: https://sso.auth.mparticle.com/\n  jwks_uri: https://sso.auth.mparticle.com/.well-known/jwks.json\n  probed: '2026-08-13'\n\
  \  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mparticle/refs/heads/main/authentication/mparticle-authentication.yml
summary_line: apiKey/http/oauth2 · 5 schemes
tags:
- Customer Data Platform
- CDP
- Analytics
- Identity Resolution
- Audience
- Data Pipeline
- Marketing Data
- Event Streaming
- Data Governance
---
