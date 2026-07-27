---
api_key_in: []
api_specs:
- filename: corelogic-au-rp-inside-auth-example.postman_collection.json
  format: json
  label: CoreLogic Australia Access API
  slug: corelogic-au-access-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/corelogic-au/refs/heads/main/collections/corelogic-au-rp-inside-auth-example.postman_collection.json
- filename: corelogic-au-sample-sandbox.postman_collection.json
  format: json
  label: CoreLogic Australia Property Details API
  slug: corelogic-au-property-details-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/corelogic-au/refs/heads/main/collections/corelogic-au-sample-sandbox.postman_collection.json
- filename: corelogic-au-sample-sandbox.postman_collection.json
  format: json
  label: CoreLogic Australia Property Services API
  slug: corelogic-au-property-services-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/corelogic-au/refs/heads/main/collections/corelogic-au-sample-sandbox.postman_collection.json
- filename: corelogic-au-sample-sandbox.postman_collection.json
  format: json
  label: CoreLogic Australia Search API
  slug: corelogic-au-search-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/corelogic-au/refs/heads/main/collections/corelogic-au-sample-sandbox.postman_collection.json
- filename: corelogic-au-sample-sandbox.postman_collection.json
  format: json
  label: CoreLogic Australia AVM API
  slug: corelogic-au-avm-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/corelogic-au/refs/heads/main/collections/corelogic-au-sample-sandbox.postman_collection.json
- filename: corelogic-au-sample-sandbox.postman_collection.json
  format: json
  label: CoreLogic Australia Auction API
  slug: corelogic-au-auction-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/corelogic-au/refs/heads/main/collections/corelogic-au-sample-sandbox.postman_collection.json
- filename: corelogic-au-sample-sandbox.postman_collection.json
  format: json
  label: CoreLogic Australia Statistics API
  slug: corelogic-au-statistics-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/corelogic-au/refs/heads/main/collections/corelogic-au-sample-sandbox.postman_collection.json
- filename: corelogic-au-sample-sandbox.postman_collection.json
  format: json
  label: CoreLogic Australia Charts API
  slug: corelogic-au-charts-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/corelogic-au/refs/heads/main/collections/corelogic-au-sample-sandbox.postman_collection.json
- filename: corelogic-au-sample-sandbox.postman_collection.json
  format: json
  label: CoreLogic Australia Property Timeline API
  slug: corelogic-au-property-timeline-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/corelogic-au/refs/heads/main/collections/corelogic-au-sample-sandbox.postman_collection.json
- filename: corelogic-au-sample-sandbox.postman_collection.json
  format: json
  label: CoreLogic Australia Content API
  slug: corelogic-au-content-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/corelogic-au/refs/heads/main/collections/corelogic-au-sample-sandbox.postman_collection.json
auth_types:
- oauth2
- openIdConnect
- http
description: ''
kind: authentication
layout: security
method: searched
name: Corelogic Au Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
- refreshToken
overview: CoreLogic Australia secures its APIs with oauth2, openIdConnect, and http across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials, authorizationCode, and refreshToken flow(s).
provider_name: CoreLogic Australia
provider_slug: corelogic-au
scheme_count: 5
schemes:
- applies_to: every Cotality Australia / New Zealand data API
  client_authentication: HTTP Basic — base64(client_id:client_secret) in the Authorization header
  flow: clientCredentials
  legacy_token_url: https://api.corelogic.asia/access/oauth/token
  name: CotalityOAuth2ClientCredentials
  sandbox_token_url: https://api-sbox.corelogic.asia/access/as/token.oauth2
  scopes_requested:
  - openid
  sources:
  - collections/corelogic-au-sample-sandbox.postman_collection.json
  - https://developer.corelogic.asia/guides/api-authentication
  token_format: JWT
  token_urls:
  - https://access.api.cotality.com.au/as/token.oauth2
  - https://access.api.cotality.com.au/oauth/token
  type: oauth2
  uat_token_url: https://access.api-uat.cotality.com.au
- endpoints:
    authorize: https://access-uat-api.corelogic.asia/access/oauth/authorize
    login: https://access-uat-api.corelogic.asia/access/login
    logout: https://access-uat-api.corelogic.asia/access/logout
    token: https://access-uat-api.corelogic.asia/access/oauth/token
    userinfo: https://access-uat-api.corelogic.asia/access/userinfo
  flow: authorizationCode
  name: CotalityOAuth2AuthorizationCode
  purpose: RP.Inside silent login / deep linking — obtains a USER token so an integrating platform can redirect a subscriber into RP Data or Property Guru without a second login. The portal is explicit that this is "not an authentication method for APIs. It is designed for user-level access and redirection, not for backend API integration."
  sources:
  - collections/corelogic-au-rp-inside-auth-example.postman_collection.json
  - https://developer.corelogic.asia/guides/application-silent-login
  type: oauth2
- flow: refreshToken
  name: CotalityOAuth2RefreshToken
  note: The portal recommends securely caching the token and refreshing prior to expiry, decoding the JWT exp claim rather than assuming a fixed lifetime.
  sources:
  - https://developer.corelogic.asia/guides/api-authentication
  type: oauth2
- claims_supported:
  - email
  - family_name
  - fax_number
  - given_name
  - mobile_number
  - personal_email
  - phone_number
  - sub
  - title
  - user_roles
  - username
  endpoints:
    authorization: https://auth.corelogic.asia/as/authorization.oauth2
    backchannel_authentication: https://auth.corelogic.asia/as/bc-auth.ciba
    device_authorization: https://auth.corelogic.asia/as/device_authz.oauth2
    end_session: https://auth.corelogic.asia/idp/init_logout.openid
    introspection: https://auth.corelogic.asia/as/introspect.oauth2
    jwks: https://auth.corelogic.asia/pf/JWKS
    registration: https://auth.corelogic.asia/as/clients.oauth2
    revocation: https://auth.corelogic.asia/as/revoke_token.oauth2
    token: https://auth.corelogic.asia/as/token.oauth2
    userinfo: https://auth.corelogic.asia/idp/userinfo.openid
  issuer: https://auth.corelogic.asia
  name: CotalityDeveloperPortalOIDC
  openIdConnectUrl: https://auth.corelogic.asia/.well-known/openid-configuration
  pkce_methods:
  - plain
  - S256
  purpose: Human login to the Cotality Developer Portal — NOT the data-API auth path. Scopes here are portal identity scopes only.
  sources:
  - well-known/corelogic-au-openid-configuration.json
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - client_secret_jwt
  - private_key_jwt
  - tls_client_auth
  - none
  type: openIdConnect
  vendor: PingFederate (Ping Identity)
- name: SSO (SAML)
  purpose: 'Application single sign-on for Cotality end-user products. The portal states plainly: "SSO is not an authentication method for APIs. It is intended for user login flows and session management." Not all applications support it yet.'
  sources:
  - https://developer.corelogic.asia/guides/application-silent-login
  type: saml2
slug: corelogic-au-authentication
source_filename: corelogic-au-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: >-\n  https://developer.corelogic.asia/guides/api-authentication (guide text compiled into the portal\n  bundle main.aefa4bad.js), https://auth.corelogic.asia/.well-known/openid-configuration,\n  collections/corelogic-au-sample-sandbox.postman_collection.json,\n  collections/corelogic-au-rp-inside-auth-example.postman_collection.json\ndocs: https://developer.corelogic.asia/guides/api-authentication\nsummary:\n  types: [oauth2, openIdConnect, http]\n  api_key_in: []\n  oauth2_flows: [clientCredentials, authorizationCode, refreshToken]\n  transport: HTTPS only, TLSv1.2 minimum\n  token_format: JWT\n  authorization_model: >-\n    Claim-based, not scope-based. The client_credentials tokens the vendor publishes in its own\n    sample collection carry scope \"openid\" only; entitlement is carried in JWT claims (roles,\n    geo_codes, authorities) provisioned against the commercial licence, so there is no data-product\n    scope surface\
  \ to request.\nverbatim:\n- >-\n  \"Our APIs use the OAuth 2.0 protocol to enable applications to request our client credential token\n  using Client ID and Client Secret.\"\n- >-\n  \"The Access Token response is a JSON Web Token (JWT) and may be decoded to obtain expiry time (a\n  Unix epoch timestamp) so that you know when to refresh the access token. Each grant_type token\n  expiry is subject to change without notice.\"\n- '\"All API requests must be made over HTTPS, with TLSv1.2 minimum.\"'\n- '\"API requests without a valid Authorization header will fail.\"'\n- '\"OAuth2 supported grant types: client_credentials, authorization_code, refresh_token.\"'\nschemes:\n- name: CotalityOAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  client_authentication: HTTP Basic — base64(client_id:client_secret) in the Authorization header\n  token_urls:\n  - https://access.api.cotality.com.au/as/token.oauth2\n  - https://access.api.cotality.com.au/oauth/token\n  sandbox_token_url:\
  \ https://api-sbox.corelogic.asia/access/as/token.oauth2\n  legacy_token_url: https://api.corelogic.asia/access/oauth/token\n  uat_token_url: https://access.api-uat.cotality.com.au\n  token_format: JWT\n  scopes_requested: [openid]\n  applies_to: every Cotality Australia / New Zealand data API\n  sources:\n  - collections/corelogic-au-sample-sandbox.postman_collection.json\n  - https://developer.corelogic.asia/guides/api-authentication\n- name: CotalityOAuth2AuthorizationCode\n  type: oauth2\n  flow: authorizationCode\n  purpose: >-\n    RP.Inside silent login / deep linking — obtains a USER token so an integrating platform can\n    redirect a subscriber into RP Data or Property Guru without a second login. The portal is\n    explicit that this is \"not an authentication method for APIs. It is designed for user-level\n    access and redirection, not for backend API integration.\"\n  endpoints:\n    authorize: https://access-uat-api.corelogic.asia/access/oauth/authorize\n    login: https://access-uat-api.corelogic.asia/access/login\n\
  \    token: https://access-uat-api.corelogic.asia/access/oauth/token\n    userinfo: https://access-uat-api.corelogic.asia/access/userinfo\n    logout: https://access-uat-api.corelogic.asia/access/logout\n  sources:\n  - collections/corelogic-au-rp-inside-auth-example.postman_collection.json\n  - https://developer.corelogic.asia/guides/application-silent-login\n- name: CotalityOAuth2RefreshToken\n  type: oauth2\n  flow: refreshToken\n  note: >-\n    The portal recommends securely caching the token and refreshing prior to expiry, decoding the\n    JWT exp claim rather than assuming a fixed lifetime.\n  sources: [https://developer.corelogic.asia/guides/api-authentication]\n- name: CotalityDeveloperPortalOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://auth.corelogic.asia/.well-known/openid-configuration\n  issuer: https://auth.corelogic.asia\n  vendor: PingFederate (Ping Identity)\n  purpose: >-\n    Human login to the Cotality Developer Portal — NOT the data-API auth path. Scopes\
  \ here are\n    portal identity scopes only.\n  endpoints:\n    authorization: https://auth.corelogic.asia/as/authorization.oauth2\n    token: https://auth.corelogic.asia/as/token.oauth2\n    userinfo: https://auth.corelogic.asia/idp/userinfo.openid\n    jwks: https://auth.corelogic.asia/pf/JWKS\n    registration: https://auth.corelogic.asia/as/clients.oauth2\n    revocation: https://auth.corelogic.asia/as/revoke_token.oauth2\n    introspection: https://auth.corelogic.asia/as/introspect.oauth2\n    end_session: https://auth.corelogic.asia/idp/init_logout.openid\n    device_authorization: https://auth.corelogic.asia/as/device_authz.oauth2\n    backchannel_authentication: https://auth.corelogic.asia/as/bc-auth.ciba\n  pkce_methods: [plain, S256]\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - client_secret_jwt\n  - private_key_jwt\n  - tls_client_auth\n  - none\n  claims_supported:\n  - email\n  - family_name\n  - fax_number\n  - given_name\n  - mobile_number\n\
  \  - personal_email\n  - phone_number\n  - sub\n  - title\n  - user_roles\n  - username\n  sources: [well-known/corelogic-au-openid-configuration.json]\n- name: SSO (SAML)\n  type: saml2\n  purpose: >-\n    Application single sign-on for Cotality end-user products. The portal states plainly: \"SSO is\n    not an authentication method for APIs. It is intended for user login flows and session\n    management.\" Not all applications support it yet.\n  sources: [https://developer.corelogic.asia/guides/application-silent-login]\ncredential_lifecycle:\n  self_serve_sandbox_client: https://developer.corelogic.asia/apps/create\n  rotate_secret: Portal \"Reset Client Secret\" action on the sandbox client\n  revoke_client: Portal \"Remove Client\" action\n  support: api.support@corelogic.com\n  production_credentials: >-\n    Not self-serve. Production and UAT credentials are provisioned only after a Cotality commercial\n    data licence is signed; the portal FAQ says an integration representative\
  \ contacts the signup\n    to discuss pricing and provisioning a full-access paid service plan.\nenvironment_binding: >-\n  Tokens are environment-bound. The portal FAQ documents the error \"Invalid token provided.\" with\n  the explanation that a token generated in UAT can only be used to make subsequent calls in UAT.\n  A sandbox client calling UAT or production returns 401 \"Restricted environment access denied.\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corelogic-au/refs/heads/main/authentication/corelogic-au-authentication.yml
summary_line: oauth2/openIdConnect/http · 5 schemes
tags:
- Real Estate
- Australia
- Property Data
- Valuation
- AVM
- PropTech
- Property Listings
- Rentals
- Auction Data
- Commercial Real Estate
- Mortgage
- Land Registry
- Cotality
- RP Data
---
