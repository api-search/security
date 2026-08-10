---
api_key_in:
- header
api_specs:
- filename: butterflymx-access-groups-api-openapi.yml
  format: yaml
  label: ButterflyMX Access groups API
  slug: butterflymx-access-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-access-groups-api-openapi.yml
- filename: butterflymx-access-logs-api-openapi.yml
  format: yaml
  label: ButterflyMX Access Logs API
  slug: butterflymx-access-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-access-logs-api-openapi.yml
- filename: butterflymx-access-points-api-openapi.yml
  format: yaml
  label: ButterflyMX Access Points API
  slug: butterflymx-access-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-access-points-api-openapi.yml
- filename: butterflymx-access-tools-api-openapi.yml
  format: yaml
  label: ButterflyMX Access Tools API
  slug: butterflymx-access-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-access-tools-api-openapi.yml
- filename: butterflymx-building-integrations-api-openapi.yml
  format: yaml
  label: ButterflyMX Building Integrations API
  slug: butterflymx-building-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-building-integrations-api-openapi.yml
- filename: butterflymx-buildings-api-openapi.yml
  format: yaml
  label: ButterflyMX Buildings API
  slug: butterflymx-buildings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-buildings-api-openapi.yml
- filename: butterflymx-calls-api-openapi.yml
  format: yaml
  label: ButterflyMX Calls API
  slug: butterflymx-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-calls-api-openapi.yml
- filename: butterflymx-devices-api-openapi.yml
  format: yaml
  label: ButterflyMX Devices API
  slug: butterflymx-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-devices-api-openapi.yml
- filename: butterflymx-door-release-requests-api-openapi.yml
  format: yaml
  label: ButterflyMX Door Release Requests API
  slug: butterflymx-door-release-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-door-release-requests-api-openapi.yml
- filename: butterflymx-keychains-api-openapi.yml
  format: yaml
  label: ButterflyMX Keychains API
  slug: butterflymx-keychains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-keychains-api-openapi.yml
- filename: butterflymx-tenant-integrations-api-openapi.yml
  format: yaml
  label: ButterflyMX Tenant Integrations API
  slug: butterflymx-tenant-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-tenant-integrations-api-openapi.yml
- filename: butterflymx-tenants-api-openapi.yml
  format: yaml
  label: ButterflyMX Tenants API
  slug: butterflymx-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-tenants-api-openapi.yml
- filename: butterflymx-units-api-openapi.yml
  format: yaml
  label: ButterflyMX Units API
  slug: butterflymx-units-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-units-api-openapi.yml
- filename: butterflymx-virtual-keys-api-openapi.yml
  format: yaml
  label: ButterflyMX Virtual Keys API
  slug: butterflymx-virtual-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-virtual-keys-api-openapi.yml
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Butterflymx Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- password
- refreshToken
overview: ButterflyMX secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, password, and refreshToken flow(s).
provider_name: ButterflyMX
provider_slug: butterflymx
scheme_count: 2
schemes:
- description: JWT necessary to make API calls
  in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/butterflymx-api-openapi.yml
  type: apiKey
- description: OAuth 2.0 authorization-code flow. The resident or admin authenticates at the ButterflyMX accounts host and the resulting authorization code is exchanged for an access token used as the API bearer token.
  flows:
  - authorizationUrl: https://accounts.butterflymx.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://accounts.butterflymx.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://accounts.butterflymx.com/oauth/token
  name: OAuth2
  sources:
  - https://apidocs.butterflymx.com/docs/authorization
  - well-known/butterflymx-openid-configuration.json
  type: oauth2
slug: butterflymx-authentication
source_filename: butterflymx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: searched\nsource: https://apidocs.butterflymx.com/docs/authorization\ndocs: https://apidocs.butterflymx.com/docs/authorization\nsummary:\n  types:\n  - oauth2\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - password\n  - refreshToken\n  note: >-\n    The published OpenAPI declares only a generic `Bearer` apiKey scheme on the `Authorization` header. The\n    real contract is OAuth 2.0 — the docs and the live authorization-server metadata at\n    accounts.butterflymx.com both document the authorization-code flow that mints that bearer token. This\n    profile records both: the spec-level scheme, and the searched OAuth 2.0 model the spec understates.\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: JWT necessary to make API calls\n  sources:\n  - openapi/butterflymx-api-openapi.yml\n- name: OAuth2\n  type: oauth2\n  description: >-\n  \
  \  OAuth 2.0 authorization-code flow. The resident or admin authenticates at the ButterflyMX accounts host\n    and the resulting authorization code is exchanged for an access token used as the API bearer token.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.butterflymx.com/oauth/authorize\n    tokenUrl: https://accounts.butterflymx.com/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://accounts.butterflymx.com/oauth/token\n  sources:\n  - https://apidocs.butterflymx.com/docs/authorization\n  - well-known/butterflymx-openid-configuration.json\nauthorization_server:\n  issuer: https://accounts.butterflymx.com\n  discovery:\n  - https://accounts.butterflymx.com/.well-known/openid-configuration\n  - https://accounts.butterflymx.com/.well-known/oauth-authorization-server\n  authorization_endpoint: https://accounts.butterflymx.com/oauth/authorize\n  token_endpoint: https://accounts.butterflymx.com/oauth/token\n  revocation_endpoint: https://accounts.butterflymx.com/oauth/revoke\n\
  \  introspection_endpoint: https://accounts.butterflymx.com/oauth/introspect\n  userinfo_endpoint: https://accounts.butterflymx.com/oauth/userinfo\n  jwks_uri: https://accounts.butterflymx.com/oauth/discovery/keys\n  grant_types_supported:\n  - authorization_code\n  - client_credentials\n  - password\n  - implicit_oidc\n  - refresh_token\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  code_challenge_methods_supported:\n  - plain\n  - S256\n  id_token_signing_alg_values_supported:\n  - RS256\ntokens:\n  access_token_lifetime_seconds: 86400\n  access_token_lifetime_note: Access token is valid for 24 hours (per the authorization guide).\n  refresh_token: >-\n    Issued alongside the access token. The docs state the refresh token does not expire and can be exchanged\n    for a new access token at any time.\n  default_redirect_uri: 'urn:ietf:wg:oauth:2.0:oob'\n  redirect_uri_note: >-\n    `urn:ietf:wg:oauth:2.0:oob` is the documented development\
  \ default; a custom redirect_uri is available on\n    request.\nsandbox:\n  issuer: https://accounts.na.sandbox.butterflymx.com\n  discovery:\n  - https://accounts.na.sandbox.butterflymx.com/.well-known/openid-configuration\n  - https://accounts.na.sandbox.butterflymx.com/.well-known/oauth-authorization-server\nx-evidence:\n- url: https://apidocs.butterflymx.com/docs/authorization.md\n  http_status: 200\n  fetched: '2026-08-08'\n- url: https://accounts.butterflymx.com/.well-known/openid-configuration\n  http_status: 200\n  fetched: '2026-08-08'\n- url: https://accounts.butterflymx.com/.well-known/oauth-authorization-server\n  http_status: 200\n  fetched: '2026-08-08'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/authentication/butterflymx-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- access-control
- physical-access
- smart-intercom
- proptech
- property-management
- multifamily
- building-automation
- visitor-management
- iot
- smart-locks
- oauth2
- webhooks
---
