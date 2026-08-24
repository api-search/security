---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: probed
name: Kevala Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Kevala secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Kevala
provider_slug: kevala
scheme_count: 2
schemes:
- description: The Kevala platform application at app.kevala.com redirects unauthenticated visitors to https://kevalaanalytics.auth0.com/authorize with response_type=code, audience=https://api.kevala.com and scope "openid profile email offline_access", i.e. the platform obtains an Auth0-issued access token for the api.kevala.com audience and calls the API with it. No client credentials, device or machine-to-machine flow is documented publicly.
  flows:
  - audience: https://api.kevala.com
    authorization_endpoint: https://kevalaanalytics.auth0.com/authorize
    authorization_server: https://kevalaanalytics.auth0.com/
    device_authorization_endpoint: https://kevalaanalytics.auth0.com/oauth/device/code
    flow: authorizationCode
    grant_types_observed:
    - authorization_code
    - refresh_token
    jwks_uri: https://kevalaanalytics.auth0.com/.well-known/jwks.json
    pkce: S256
    registration_endpoint: https://kevalaanalytics.auth0.com/oidc/register
    revocation_endpoint: https://kevalaanalytics.auth0.com/oauth/revoke
    scopes_requested_by_platform:
    - openid
    - profile
    - email
    - offline_access
    sources:
    - well-known/kevala-auth0-openid-configuration.json
    token_endpoint: https://kevalaanalytics.auth0.com/oauth/token
    userinfo_endpoint: https://kevalaanalytics.auth0.com/userinfo
  name: oauth2
  type: oauth2
- description: OIDC discovery is live on the company's Auth0 tenant (HTTP 200) and advertises S256 PKCE, private_key_jwt / client_secret_basic / client_secret_post / none client authentication, and the standard OIDC scope set. This is Auth0-provided infrastructure configured by Kevala, not a document served from a kevala.com host.
  name: openIdConnect
  openIdConnectUrl: https://kevalaanalytics.auth0.com/.well-known/openid-configuration
  type: openIdConnect
slug: kevala-authentication
source_filename: kevala-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: >-\n  https://app.kevala.com/ authorize redirect (observed 2026-08-23) +\n  https://kevalaanalytics.auth0.com/.well-known/openid-configuration (HTTP 200) +\n  anonymous probes of https://api.kevala.com/der/ (HTTP 403)\ndocs: null\ndocs_note: >-\n  Kevala publishes no public authentication page or developer reference. Everything below was\n  observed directly from the login redirect, the Auth0 tenant discovery document, and the API's own\n  anonymous responses. No credential values are recorded.\nsummary:\n  types: [oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  identity_provider: Auth0 (tenant kevalaanalytics.auth0.com)\n  api_audience: https://api.kevala.com\nschemes:\n- name: oauth2\n  type: oauth2\n  description: >-\n    The Kevala platform application at app.kevala.com redirects unauthenticated visitors to\n    https://kevalaanalytics.auth0.com/authorize with response_type=code,\n    audience=https://api.kevala.com\
  \ and scope \"openid profile email offline_access\", i.e. the\n    platform obtains an Auth0-issued access token for the api.kevala.com audience and calls the API\n    with it. No client credentials, device or machine-to-machine flow is documented publicly.\n  flows:\n  - flow: authorizationCode\n    authorization_server: https://kevalaanalytics.auth0.com/\n    authorization_endpoint: https://kevalaanalytics.auth0.com/authorize\n    token_endpoint: https://kevalaanalytics.auth0.com/oauth/token\n    userinfo_endpoint: https://kevalaanalytics.auth0.com/userinfo\n    jwks_uri: https://kevalaanalytics.auth0.com/.well-known/jwks.json\n    revocation_endpoint: https://kevalaanalytics.auth0.com/oauth/revoke\n    device_authorization_endpoint: https://kevalaanalytics.auth0.com/oauth/device/code\n    registration_endpoint: https://kevalaanalytics.auth0.com/oidc/register\n    pkce: S256\n    grant_types_observed: [authorization_code, refresh_token]\n    scopes_requested_by_platform: [openid, profile,\
  \ email, offline_access]\n    audience: https://api.kevala.com\n    sources: [well-known/kevala-auth0-openid-configuration.json]\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://kevalaanalytics.auth0.com/.well-known/openid-configuration\n  description: >-\n    OIDC discovery is live on the company's Auth0 tenant (HTTP 200) and advertises S256 PKCE,\n    private_key_jwt / client_secret_basic / client_secret_post / none client authentication, and\n    the standard OIDC scope set. This is Auth0-provided infrastructure configured by Kevala, not a\n    document served from a kevala.com host.\nobserved_behaviour:\n- url: https://api.kevala.com/der/\n  status: 403\n  body: '{\"detail\":\"Authentication credentials were not provided.\"}'\n  note: Django REST Framework rejection; no WWW-Authenticate challenge header is returned.\n- url: https://api.kevala.com/der/openapi/\n  status: 403\n  content_type: application/vnd.oai.openapi\n  note: >-\n    The OpenAPI document\
  \ itself is credential-gated. The endpoint exists and negotiates the OpenAPI\n    media type, but anonymous callers receive the DRF not_authenticated envelope.\ngaps:\n- No public developer signup or key-issuance path; access follows a subscription/Order Form.\n- No documented service-to-service (client credentials) flow, token lifetime, or refresh guidance.\n- No WWW-Authenticate header on 401/403, so an agent cannot discover the authorization server from\n  the API response alone.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kevala/refs/heads/main/authentication/kevala-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Energy
- Electricity
- Electric Grid
- Grid Analytics
- Distributed Energy Resources
- Utilities
- Geospatial
- Analytics
- Carbon Accounting
- Electric Vehicles
- Sustainability
---
