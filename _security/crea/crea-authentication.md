---
api_key_in: []
api_specs:
- filename: crea-realtor-ca-ddf-web-api-openapi.json
  format: json
  label: REALTOR.ca DDF Web API
  slug: realtor-ca-ddf-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crea/refs/heads/main/openapi/crea-realtor-ca-ddf-web-api-openapi.json
- filename: crea-realtor-ca-ddf-web-api-openapi.json
  format: json
  label: REALTOR.ca DDF Lead API
  slug: realtor-ca-ddf-lead-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crea/refs/heads/main/openapi/crea-realtor-ca-ddf-web-api-openapi.json
- filename: crea-realtor-ca-board-api-openapi.json
  format: json
  label: REALTOR.ca Board API
  slug: realtor-ca-board-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crea/refs/heads/main/openapi/crea-realtor-ca-board-api-openapi.json
auth_types:
- oauth2
- openIdConnect
description: Every REALTOR.ca API is fronted by a single Duende/IdentityServer deployment at identity.crea.ca. Neither OpenAPI document declares a securityScheme - the derived pass over openapi/ found zero schemes across all three specs - so this profile is taken from the provider's own Authorization documentation and from the anonymous OpenID Connect discovery document, both harvested 2026-07-26. The only supported machine flow is OAuth 2.0 client credentials; credentials are issued by CREA and there is no self-serve path.
kind: authentication
layout: security
method: searched
name: Crea Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: CREA (REALTOR.ca) secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: CREA (REALTOR.ca)
provider_slug: crea
scheme_count: 2
schemes:
- applies_to:
  - crea:realtor-ca-ddf-web-api
  - crea:realtor-ca-ddf-lead-api
  - crea:realtor-ca-board-api
  client_authentication:
  - client_secret_basic
  - client_secret_post
  flow: clientCredentials
  name: CREA IdentityServer client credentials
  parameters:
    client_id: The username of your Destination (DDF data feed) or Board
    client_secret: The password of your Destination or Board
    grant_type: client_credentials
    scope: DDFApi_Read (DDF Web API and Lead API) or BoardDataApi.read (Board API)
  request_encoding: application/x-www-form-urlencoded
  response_fields:
    access_token: The bearer token
    expires_in: 3600 by default; the token is NOT sliding, a new token must be requested after one hour
    scope: Echoes the requested scope
    token_type: Bearer
  sources:
  - https://ddfapi-docs.realtor.ca/
  - https://boardapi-docs.realtor.ca/
  token_placement: Authorization header, "Bearer <access_token>"
  token_url: https://identity.crea.ca/connect/token
  type: oauth2
- authorization_endpoint: https://identity.crea.ca/connect/authorize
  backchannel_logout_supported: true
  claims_supported:
  - sub
  - destinationid
  code_challenge_methods_supported:
  - plain
  - S256
  device_authorization_endpoint: https://identity.crea.ca/connect/deviceauthorization
  end_session_endpoint: https://identity.crea.ca/connect/endsession
  frontchannel_logout_supported: true
  grant_types_supported:
  - authorization_code
  - client_credentials
  - refresh_token
  - implicit
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:openid:params:grant-type:ciba
  id_token_signing_alg_values_supported:
  - RS256
  introspection_endpoint: https://identity.crea.ca/connect/introspect
  issuer: https://identity.crea.ca
  jwks_uri: https://identity.crea.ca/.well-known/openid-configuration/jwks
  name: CREA OpenID Connect provider
  note: The discovery document advertises far more than the documented APIs use. Only client_credentials is documented for DDF and Board; authorization_code, implicit, device code and CIBA are advertised by the shared identity server and are presumably used by CREA's member-facing products (DDF Dashboard, WEBForms, Offer Management). The "destinationid" claim is what scopes a DDF token to a data feed.
  openid_configuration: https://identity.crea.ca/.well-known/openid-configuration
  pushed_authorization_request_endpoint: https://identity.crea.ca/connect/par
  require_pushed_authorization_requests: false
  revocation_endpoint: https://identity.crea.ca/connect/revocation
  subject_types_supported:
  - public
  token_endpoint: https://identity.crea.ca/connect/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
  userinfo_endpoint: https://identity.crea.ca/connect/userinfo
slug: crea-authentication
source_filename: crea-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: https://ddfapi-docs.realtor.ca/ (Authorization section), https://boardapi-docs.realtor.ca/ (Authorization section)\ndocs: https://ddfapi-docs.realtor.ca/#section/Authorization\ndiscovery: https://identity.crea.ca/.well-known/openid-configuration\ndescription: >-\n  Every REALTOR.ca API is fronted by a single Duende/IdentityServer deployment at\n  identity.crea.ca. Neither OpenAPI document declares a securityScheme - the derived pass over\n  openapi/ found zero schemes across all three specs - so this profile is taken from the\n  provider's own Authorization documentation and from the anonymous OpenID Connect discovery\n  document, both harvested 2026-07-26. The only supported machine flow is OAuth 2.0 client\n  credentials; credentials are issued by CREA and there is no self-serve path.\nsummary:\n  types: [oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [clientCredentials]\n  spec_declared_schemes: 0\n  self_serve_signup:\
  \ false\nschemes:\n- name: CREA IdentityServer client credentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://identity.crea.ca/connect/token\n  request_encoding: application/x-www-form-urlencoded\n  client_authentication: [client_secret_basic, client_secret_post]\n  parameters:\n    client_id: The username of your Destination (DDF data feed) or Board\n    client_secret: The password of your Destination or Board\n    grant_type: client_credentials\n    scope: DDFApi_Read (DDF Web API and Lead API) or BoardDataApi.read (Board API)\n  response_fields:\n    access_token: The bearer token\n    expires_in: 3600 by default; the token is NOT sliding, a new token must be requested after one hour\n    token_type: Bearer\n    scope: Echoes the requested scope\n  token_placement: Authorization header, \"Bearer <access_token>\"\n  applies_to:\n  - crea:realtor-ca-ddf-web-api\n  - crea:realtor-ca-ddf-lead-api\n  - crea:realtor-ca-board-api\n  sources: [https://ddfapi-docs.realtor.ca/,\
  \ https://boardapi-docs.realtor.ca/]\n- name: CREA OpenID Connect provider\n  type: openIdConnect\n  issuer: https://identity.crea.ca\n  openid_configuration: https://identity.crea.ca/.well-known/openid-configuration\n  jwks_uri: https://identity.crea.ca/.well-known/openid-configuration/jwks\n  authorization_endpoint: https://identity.crea.ca/connect/authorize\n  token_endpoint: https://identity.crea.ca/connect/token\n  userinfo_endpoint: https://identity.crea.ca/connect/userinfo\n  introspection_endpoint: https://identity.crea.ca/connect/introspect\n  revocation_endpoint: https://identity.crea.ca/connect/revocation\n  end_session_endpoint: https://identity.crea.ca/connect/endsession\n  device_authorization_endpoint: https://identity.crea.ca/connect/deviceauthorization\n  pushed_authorization_request_endpoint: https://identity.crea.ca/connect/par\n  require_pushed_authorization_requests: false\n  grant_types_supported: [authorization_code, client_credentials, refresh_token, implicit, 'urn:ietf:params:oauth:grant-type:device_code',\
  \ 'urn:openid:params:grant-type:ciba']\n  code_challenge_methods_supported: [plain, S256]\n  id_token_signing_alg_values_supported: [RS256]\n  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post]\n  claims_supported: [sub, destinationid]\n  subject_types_supported: [public]\n  frontchannel_logout_supported: true\n  backchannel_logout_supported: true\n  note: >-\n    The discovery document advertises far more than the documented APIs use. Only\n    client_credentials is documented for DDF and Board; authorization_code, implicit, device\n    code and CIBA are advertised by the shared identity server and are presumably used by\n    CREA's member-facing products (DDF Dashboard, WEBForms, Offer Management). The\n    \"destinationid\" claim is what scopes a DDF token to a data feed.\ncredential_issuance:\n  self_serve: false\n  process: >-\n    A REALTOR opts a data feed in through the DDF Dashboard on CREA's member portal\n    (ddf.realtor.ca, SSO via sso.realtor.ca).\
  \ A third-party developer must enter a data access\n    agreement with CREA as a Technology Provider operating a National Pool Website or Member\n    Website on behalf of that opted-in member. client_id and client_secret are then provided\n    by CREA. Board API credentials are provided by CREA to member boards.\n  gotchas:\n  - An inactive data feed returns no access token at all, rather than an error explaining why.\n  - Technology Provider accounts get their own credentials that merge every linked feed into one unified dataset.\n  - CREA recommends server-to-server token use only; client-to-server token requests are called out as a security risk.\ntransport_security:\n  min_tls: '1.2'\n  https_required: true\n  source: Release note 2023-01-31 - \"Update to support minimum TLS version 1.2 enforcing all incoming requests to be HTTPS.\"\nrelated:\n  scopes: scopes/crea-scopes.yml\n  well_known: well-known/crea-well-known.yml\n  conventions: conventions/crea-conventions.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crea/refs/heads/main/authentication/crea-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Real Estate
- Canada
- Property Listings
- MLS
- IDX
- RESO
- OData
- Industry Body
- PropTech
- Data Syndication
---
