---
api_key_in: []
api_specs:
- filename: rose-rocket-boards-api-openapi.yml
  format: yaml
  label: Rose Rocket Boards API
  slug: rose-rocket-boards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rose-rocket/refs/heads/main/openapi/rose-rocket-boards-api-openapi.yml
- filename: rose-rocket-events-api-openapi.yml
  format: yaml
  label: Rose Rocket Events API
  slug: rose-rocket-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rose-rocket/refs/heads/main/openapi/rose-rocket-events-api-openapi.yml
- filename: rose-rocket-object-records-api-openapi.yml
  format: yaml
  label: Rose Rocket Object Records API
  slug: rose-rocket-object-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rose-rocket/refs/heads/main/openapi/rose-rocket-object-records-api-openapi.yml
- filename: rose-rocket-user-groups-api-openapi.yml
  format: yaml
  label: Rose Rocket User Groups API
  slug: rose-rocket-user-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rose-rocket/refs/heads/main/openapi/rose-rocket-user-groups-api-openapi.yml
auth_types: []
description: 'Rose Rocket authenticates every Platform API request with an OAuth 2.0 bearer access token issued by a.roserocket.com, an Auth0-hosted authorization server that publishes a full OIDC discovery document. Two documented paths exist: the authorization-code flow for applications acting on behalf of an end user, and a client-credentials "service account" flow for machine-to-machine access. NOTE THE GAP: the published OpenAPI (openapi/rose-rocket-platform-model-api.json) declares NO components.securitySchemes and NO security requirement on any of its 19 operations. The auth model below is real but lives only in prose — a client generated from the spec alone would emit unauthenticated requests. The overlay in overlays/ records this as our enhancement without mutating the original.'
kind: authentication
layout: security
method: searched
name: Rose Rocket Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rose Rocket declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Rose Rocket
provider_slug: rose-rocket
scheme_count: 2
schemes:
- audience: https://roserocket.com
  docs: https://roserocket.readme.io/docs/rose-rocket-api-oauth-20-authentication-guide
  flow: authorizationCode
  header: 'Authorization: Bearer <access_token>'
  id: oauth2-authorization-code
  in: header
  note: End-user consent flow. The user authenticates against a social connection or a customer-configured third-party IdP (the guide names Azure Active Directory); configuring an IdP requires contacting Rose Rocket.
  parameters:
  - audience
  - response_type=code
  - client_id
  - redirect_uri
  - scope
  - state
  pkce: supported (code_challenge_methods_supported = S256, plain)
  scopes_requested:
  - offline_access
  - email
  - profile
  type: oauth2
- audience: https://roserocket.com
  docs: https://roserocket.readme.io/docs/rose-rocket-api-oauth-20-authentication-guide
  extra_parameters:
  - org_id
  - user_id
  flow: clientCredentials
  header: 'Authorization: Bearer <access_token>'
  id: oauth2-client-credentials-service-account
  in: header
  note: Machine-to-machine. A Service Account user is created under the org and bound to the OAuth application; the token request carries org_id and the service account's user_id alongside client_id/client_secret. The service account defaults to the Manager role — see the roles model in https://roserocket.readme.io/docs/roles-and-permissions.
  type: oauth2
slug: rose-rocket-authentication
source_filename: rose-rocket-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: >-\n  https://roserocket.readme.io/docs/rose-rocket-api-oauth-20-authentication-guide,\n  https://roserocket.readme.io/docs/application-lifecycle-management,\n  https://roserocket.readme.io/docs/getting-started, and the live discovery\n  document at https://a.roserocket.com/.well-known/openid-configuration (HTTP 200,\n  probed 2026-08-26).\ndescription: >-\n  Rose Rocket authenticates every Platform API request with an OAuth 2.0 bearer\n  access token issued by a.roserocket.com, an Auth0-hosted authorization server\n  that publishes a full OIDC discovery document. Two documented paths exist:\n  the authorization-code flow for applications acting on behalf of an end user,\n  and a client-credentials \"service account\" flow for machine-to-machine access.\n  NOTE THE GAP: the published OpenAPI (openapi/rose-rocket-platform-model-api.json)\n  declares NO components.securitySchemes and NO security requirement on any of its\n  19\
  \ operations. The auth model below is real but lives only in prose — a client\n  generated from the spec alone would emit unauthenticated requests. The overlay\n  in overlays/ records this as our enhancement without mutating the original.\nauthorization_server: https://a.roserocket.com/\ndiscovery:\n  openid_configuration: https://a.roserocket.com/.well-known/openid-configuration\n  oauth_authorization_server: https://a.roserocket.com/.well-known/oauth-authorization-server\n  jwks_uri: https://a.roserocket.com/.well-known/jwks.json\n  saved: well-known/rose-rocket-openid-configuration.json\nendpoints:\n  authorization: https://a.roserocket.com/authorize\n  token: https://a.roserocket.com/oauth/token\n  userinfo: https://a.roserocket.com/userinfo\n  revocation: https://a.roserocket.com/oauth/revoke\n  device_authorization: https://a.roserocket.com/oauth/device/code\n  registration: https://a.roserocket.com/oidc/register\n  end_session: https://a.roserocket.com/oidc/logout\nschemes:\n  -\
  \ id: oauth2-authorization-code\n    type: oauth2\n    flow: authorizationCode\n    in: header\n    header: 'Authorization: Bearer <access_token>'\n    audience: https://roserocket.com\n    scopes_requested: [offline_access, email, profile]\n    parameters: [audience, response_type=code, client_id, redirect_uri, scope, state]\n    pkce: supported (code_challenge_methods_supported = S256, plain)\n    docs: https://roserocket.readme.io/docs/rose-rocket-api-oauth-20-authentication-guide\n    note: >-\n      End-user consent flow. The user authenticates against a social connection or\n      a customer-configured third-party IdP (the guide names Azure Active Directory);\n      configuring an IdP requires contacting Rose Rocket.\n  - id: oauth2-client-credentials-service-account\n    type: oauth2\n    flow: clientCredentials\n    in: header\n    header: 'Authorization: Bearer <access_token>'\n    audience: https://roserocket.com\n    extra_parameters: [org_id, user_id]\n    docs: https://roserocket.readme.io/docs/rose-rocket-api-oauth-20-authentication-guide\n\
  \    note: >-\n      Machine-to-machine. A Service Account user is created under the org and bound\n      to the OAuth application; the token request carries org_id and the service\n      account's user_id alongside client_id/client_secret. The service account\n      defaults to the Manager role — see the roles model in\n      https://roserocket.readme.io/docs/roles-and-permissions.\ntoken:\n  type: JWT bearer\n  lifetime: >-\n    Short-lived and deliberately unspecified. The Authentication Guide states\n    sessions \"may expire sooner than expected\" and that the timing \"may vary as we\n    continuously improve our security systems\"; clients must detect 401 and refresh.\n    A separate Getting Started page states access tokens last a maximum of 24 hours.\n  refresh: >-\n    grant_type=refresh_token against https://a.roserocket.com/oauth/token with\n    client_id, client_secret, refresh_token and org_id.\n  expiry_signal: HTTP 401\ncredentials:\n  issuance: >-\n    NOT self-serve. Credentials\
  \ are provisioned by Rose Rocket: existing customers\n    obtain API access through their account representative; independent software\n    vendors go through the Partnership team. An OAuth application is then created\n    in-product under Settings > API Settings > Applications > OAuth Applications.\n  fields: [client_id, client_secret, redirect_uris]\n  rotation: >-\n    Client secrets are rotatable in-product (Rotate Secret). Rotation invalidates the\n    previous secret immediately with no overlap window.\n    Source: https://roserocket.readme.io/docs/application-lifecycle-management\n  deletion: >-\n    Deleting an OAuth application is irreversible and immediately revokes that\n    application's API access.\nmtls: false\napi_keys: false\napi_keys_note: No API-key scheme is documented. All access is OAuth 2.0 bearer.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rose-rocket/refs/heads/main/authentication/rose-rocket-authentication.yml
summary_line: 2 schemes
tags:
- Transportation
- Logistics
- Freight
- Trucking
- Transportation Management System
- Supply Chain
- Dispatch
- Webhook
- Authentication
- Canada
---
