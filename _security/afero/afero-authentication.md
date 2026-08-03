---
api_key_in: []
api_specs:
- filename: afero-cloud-api-openapi.yml
  format: yaml
  label: Afero Cloud API
  slug: cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afero/refs/heads/main/openapi/_original/afero-cloud-api-openapi.yml
- filename: afero-authentication-api-openapi.yml
  format: yaml
  label: Afero Cloud Authentication API
  slug: authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afero/refs/heads/main/openapi/afero-authentication-api-openapi.yml
- filename: afero-users-api-openapi.yml
  format: yaml
  label: Afero Cloud Users API
  slug: users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afero/refs/heads/main/openapi/afero-users-api-openapi.yml
- filename: afero-devices-api-openapi.yml
  format: yaml
  label: Afero Cloud Devices API
  slug: devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afero/refs/heads/main/openapi/afero-devices-api-openapi.yml
- filename: afero-ota-api-openapi.yml
  format: yaml
  label: Afero Cloud OTA Firmware API
  slug: ota-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afero/refs/heads/main/openapi/afero-ota-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Afero Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Afero secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Afero
provider_slug: afero
scheme_count: 2
schemes:
- description: HTTP Basic client authentication on the token endpoint. The header value is the string `Basic ` followed by the Base64 encoding of `<OAuth Client ID>:<OAuth Client Secret>`. Both credentials are issued to a partner and viewed in the Afero Profile Editor under VIEW > ACCOUNT INFO. Afero warns that developer credentials obtained through the Profile Editor must not be used in production applications.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/afero-authentication-api-openapi.yml
  type: http
  used_on:
  - POST /oauth/token
- description: 'The OAuth 2.0 access token returned by POST /oauth/token, sent as `Authorization: Bearer <access_token>`. The token is issued for an end-user and is used to authenticate requests on that user''s behalf. It expires — the docs state approximately four hours and the response carries expires_in in seconds. An expired or missing token returns HTTP 401 with error `unauthorized`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/afero-devices-api-openapi.yml
  - openapi/afero-ota-api-openapi.yml
  - openapi/afero-users-api-openapi.yml
  type: http
  used_on:
  - Every /v1/ operation (users, devices, OTA)
slug: afero-authentication
source_filename: afero-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: openapi/afero-authentication-api-openapi.yml, openapi/afero-devices-api-openapi.yml,\n  openapi/afero-ota-api-openapi.yml, openapi/afero-users-api-openapi.yml\ndocs: https://afero-docs.readthedocs.io/en/latest/API-OAuthEndpoints/\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - password\n  token_endpoint: https://api.afero.io/oauth/token\n  client_authentication: http-basic\n  token_transport: 'Authorization: Bearer <access_token>'\n  token_lifetime: Approximately four hours; exact value returned in expires_in (seconds).\n  refresh_token: Not documented — re-run the password grant when the token expires.\n  scopes_documented: false\n  standards:\n  - RFC 6749 (cited directly by Afero in the OTA API prerequisites)\n  - RFC 6750 bearer token usage\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  used_on:\n  - POST /oauth/token\n  description: 'HTTP Basic client authentication on the token endpoint.\
  \ The header value is the\n    string `Basic ` followed by the Base64 encoding of `<OAuth Client ID>:<OAuth Client Secret>`.\n    Both credentials are issued to a partner and viewed in the Afero Profile Editor under\n    VIEW > ACCOUNT INFO. Afero warns that developer credentials obtained through the Profile\n    Editor must not be used in production applications.'\n  sources:\n  - openapi/afero-authentication-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  used_on:\n  - Every /v1/ operation (users, devices, OTA)\n  description: 'The OAuth 2.0 access token returned by POST /oauth/token, sent as\n    `Authorization: Bearer <access_token>`. The token is issued for an end-user and is used to\n    authenticate requests on that user''s behalf. It expires — the docs state approximately four\n    hours and the response carries expires_in in seconds. An expired or missing token returns\n    HTTP 401 with error `unauthorized`.'\n  sources:\n  - openapi/afero-devices-api-openapi.yml\n\
  \  - openapi/afero-ota-api-openapi.yml\n  - openapi/afero-users-api-openapi.yml\nflow:\n  grant_type: password\n  request:\n    method: POST\n    url: https://api.afero.io/oauth/token\n    headers:\n      Content-Type: application/x-www-form-urlencoded\n      Accept: application/json\n      Authorization: Basic <base64(clientId:clientSecret)>\n    body_fields:\n    - username (the Afero account email address)\n    - password\n    - grant_type=password\n  response_fields:\n  - access_token\n  - token_type (bearer)\n  - expires_in (seconds)\n  - scope\n  observed_scope_value: partner account\nauthorization_model:\n  note: 'Afero has no OAuth scope reference page and does not document scope-based authorization.\n    Authorization is enforced through account and partner PRIVILEGE objects returned by\n    GET /v1/users/me rather than through token scopes.'\n  account_privileges:\n  - canWrite\n  - owner\n  partner_privileges:\n  - inviteUsers\n  - manageDeviceProfiles\n  - owner\n  - viewDeviceInfo\n\
  \  source: https://afero-docs.readthedocs.io/en/latest/API-UserEndpoints/\ndiscovery:\n  openid_configuration: 404 at https://api.afero.io/.well-known/openid-configuration\n  oauth_authorization_server: 404 at https://api.afero.io/.well-known/oauth-authorization-server\n  note: Afero publishes no OAuth or OIDC discovery metadata; the token endpoint is documented in\n    prose only.\ngaps:\n- No authorization_code or client_credentials flow — only the RFC 6749 resource owner password\n  credentials grant, which requires the partner application to handle end-user passwords directly.\n- No documented refresh token.\n- No OAuth scopes are published, so scopes/ is not emitted for this provider.\n- No PKCE, no token revocation and no token introspection endpoint documented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/afero/refs/heads/main/authentication/afero-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Internet of Things
- IoT Platform
- Connected Devices
- Device Management
- Firmware
- Over-the-Air Updates
- Bluetooth Low Energy
- Embedded Security
- Hardware
---
