---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Wawanesa Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- refreshToken
- password
- deviceCode
- clientCredentials
overview: Wawanesa Insurance secures its APIs with oauth2 and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, refreshToken, password, deviceCode, and clientCredentials flow(s).
provider_name: Wawanesa Insurance
provider_slug: wawanesa
scheme_count: 3
schemes:
- authorizationUrl: https://login.brokerplatform.wawanesa.com/oauth2/v1/authorize
  deviceAuthorizationEndpoint: https://login.brokerplatform.wawanesa.com/oauth2/v1/device/authorize
  dpopSigningAlgs:
  - RS256
  - RS384
  - RS512
  - ES256
  - ES384
  - ES512
  grantTypes:
  - authorization_code
  - implicit
  - refresh_token
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  idTokenSigningAlgs:
  - RS256
  introspectionEndpoint: https://login.brokerplatform.wawanesa.com/oauth2/v1/introspect
  issuer: https://login.brokerplatform.wawanesa.com
  jwksUri: https://login.brokerplatform.wawanesa.com/oauth2/v1/keys
  name: BrokerPlatformOkta
  openIdConnectUrl: https://login.brokerplatform.wawanesa.com/.well-known/openid-configuration
  pkce:
  - S256
  provider: Okta
  registrationEndpoint: https://login.brokerplatform.wawanesa.com/oauth2/v1/clients
  revocationEndpoint: https://login.brokerplatform.wawanesa.com/oauth2/v1/revoke
  role: broker identity provider for the Wawanesa Broker Platform
  scopeCount: 7
  scopes_note: stock OIDC scopes (openid, email, profile, address, phone, offline_access, groups)
  sources:
  - well-known/wawanesa-brokerplatform-login-openid-configuration.json
  tokenEndpointAuthMethods:
  - client_secret_basic
  - client_secret_post
  - client_secret_jwt
  - private_key_jwt
  - none
  tokenUrl: https://login.brokerplatform.wawanesa.com/oauth2/v1/token
  type: openIdConnect
  userinfoUrl: https://login.brokerplatform.wawanesa.com/oauth2/v1/userinfo
- grantTypes:
  - authorization_code
  - implicit
  - refresh_token
  - password
  - client_credentials
  - urn:ietf:params:oauth:grant-type:device_code
  issuer: https://login.brokerplatform.wawanesa.com
  metadata: https://login.brokerplatform.wawanesa.com/.well-known/oauth-authorization-server
  name: BrokerPlatformOktaOrgAuthorizationServer
  role: Okta org authorization server (platform administration, not an insurance API)
  scopeCount: 83
  scopes_note: all 83 advertised scopes are Okta platform management scopes (okta.users.*, okta.apps.*, okta.groups.*, ...), not Wawanesa insurance scopes
  sources:
  - well-known/wawanesa-brokerplatform-login-oauth-authorization-server.json
  spec: RFC 8414
  type: oauth2
- authorizationUrl: https://brokerplatform.wawanesa.com/services/oauth2/authorize
  endSessionEndpoint: https://brokerplatform.wawanesa.com/services/auth/idp/oidc/logout
  introspectionEndpoint: https://brokerplatform.wawanesa.com/services/oauth2/introspect
  issuer: https://brokerplatform.wawanesa.com
  jwksUri: https://brokerplatform.wawanesa.com/id/keys
  name: BrokerPlatformSalesforce
  openIdConnectUrl: https://brokerplatform.wawanesa.com/.well-known/openid-configuration
  provider: Salesforce Experience Cloud
  registrationEndpoint: https://brokerplatform.wawanesa.com/services/oauth2/register
  revocationEndpoint: https://brokerplatform.wawanesa.com/services/oauth2/revoke
  role: Salesforce Experience Cloud OIDC for the Broker Platform community
  scopeCount: 36
  scopes_note: stock Salesforce platform scopes (api, web, chatter_api, cdp_*, ...)
  sources:
  - well-known/wawanesa-brokerplatform-openid-configuration.json
  tokenEndpointAuthMethods:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  tokenUrl: https://brokerplatform.wawanesa.com/services/oauth2/token
  type: openIdConnect
  userinfoUrl: https://brokerplatform.wawanesa.com/services/oauth2/userinfo
slug: wawanesa-authentication
source_filename: wawanesa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: >-\n  live anonymous fetch of the OpenID Connect / OAuth 2.0 discovery documents on\n  the Wawanesa Broker Platform hosts (2026-07-25), plus CSIO's published API\n  Security Standards certification for Wawanesa\ndocs: https://login.brokerplatform.wawanesa.com/.well-known/openid-configuration\nnote: >-\n  Wawanesa publishes no OpenAPI, so this profile is not derived from a spec. It\n  is harvested from the only authentication metadata Wawanesa exposes on the\n  open internet: the identity providers in front of the gated broker channel.\n  These documents govern how a human broker signs in to the Broker Platform.\n  There is NO documented machine-to-machine credential, client-registration\n  path, or token endpoint for a third-party developer to call a Wawanesa\n  insurance API — onboarding runs through a Wawanesa Business Development\n  representative. The business-level auth model for the broker APIs is defined\n  by CSIO's\
  \ API Security Standards (a standard authentication and authorization\n  API model for Canadian carriers and Broker Management System vendors), which\n  Wawanesa was certified against on 2024-10-29; the standard itself is\n  member-gated at csio.com and is not reproduced here.\nsummary:\n  types: [oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, implicit, refreshToken, password, deviceCode, clientCredentials]\n  public_developer_credential: false\n  self_serve_signup: false\n  onboarding: contact a Wawanesa Business Development representative (broker channel only)\nschemes:\n- name: BrokerPlatformOkta\n  type: openIdConnect\n  role: broker identity provider for the Wawanesa Broker Platform\n  provider: Okta\n  openIdConnectUrl: https://login.brokerplatform.wawanesa.com/.well-known/openid-configuration\n  issuer: https://login.brokerplatform.wawanesa.com\n  authorizationUrl: https://login.brokerplatform.wawanesa.com/oauth2/v1/authorize\n  tokenUrl: https://login.brokerplatform.wawanesa.com/oauth2/v1/token\n\
  \  userinfoUrl: https://login.brokerplatform.wawanesa.com/oauth2/v1/userinfo\n  jwksUri: https://login.brokerplatform.wawanesa.com/oauth2/v1/keys\n  registrationEndpoint: https://login.brokerplatform.wawanesa.com/oauth2/v1/clients\n  introspectionEndpoint: https://login.brokerplatform.wawanesa.com/oauth2/v1/introspect\n  revocationEndpoint: https://login.brokerplatform.wawanesa.com/oauth2/v1/revoke\n  deviceAuthorizationEndpoint: https://login.brokerplatform.wawanesa.com/oauth2/v1/device/authorize\n  grantTypes:\n  - authorization_code\n  - implicit\n  - refresh_token\n  - password\n  - urn:ietf:params:oauth:grant-type:device_code\n  tokenEndpointAuthMethods:\n  - client_secret_basic\n  - client_secret_post\n  - client_secret_jwt\n  - private_key_jwt\n  - none\n  pkce: [S256]\n  dpopSigningAlgs: [RS256, RS384, RS512, ES256, ES384, ES512]\n  idTokenSigningAlgs: [RS256]\n  scopeCount: 7\n  scopes_note: stock OIDC scopes (openid, email, profile, address, phone, offline_access, groups)\n \
  \ sources: [well-known/wawanesa-brokerplatform-login-openid-configuration.json]\n- name: BrokerPlatformOktaOrgAuthorizationServer\n  type: oauth2\n  role: Okta org authorization server (platform administration, not an insurance API)\n  metadata: https://login.brokerplatform.wawanesa.com/.well-known/oauth-authorization-server\n  spec: RFC 8414\n  issuer: https://login.brokerplatform.wawanesa.com\n  grantTypes:\n  - authorization_code\n  - implicit\n  - refresh_token\n  - password\n  - client_credentials\n  - urn:ietf:params:oauth:grant-type:device_code\n  scopeCount: 83\n  scopes_note: >-\n    all 83 advertised scopes are Okta platform management scopes (okta.users.*,\n    okta.apps.*, okta.groups.*, ...), not Wawanesa insurance scopes\n  sources: [well-known/wawanesa-brokerplatform-login-oauth-authorization-server.json]\n- name: BrokerPlatformSalesforce\n  type: openIdConnect\n  role: Salesforce Experience Cloud OIDC for the Broker Platform community\n  provider: Salesforce Experience\
  \ Cloud\n  openIdConnectUrl: https://brokerplatform.wawanesa.com/.well-known/openid-configuration\n  issuer: https://brokerplatform.wawanesa.com\n  authorizationUrl: https://brokerplatform.wawanesa.com/services/oauth2/authorize\n  tokenUrl: https://brokerplatform.wawanesa.com/services/oauth2/token\n  userinfoUrl: https://brokerplatform.wawanesa.com/services/oauth2/userinfo\n  jwksUri: https://brokerplatform.wawanesa.com/id/keys\n  registrationEndpoint: https://brokerplatform.wawanesa.com/services/oauth2/register\n  introspectionEndpoint: https://brokerplatform.wawanesa.com/services/oauth2/introspect\n  revocationEndpoint: https://brokerplatform.wawanesa.com/services/oauth2/revoke\n  endSessionEndpoint: https://brokerplatform.wawanesa.com/services/auth/idp/oidc/logout\n  tokenEndpointAuthMethods:\n  - client_secret_post\n  - client_secret_basic\n  - private_key_jwt\n  scopeCount: 36\n  scopes_note: stock Salesforce platform scopes (api, web, chatter_api, cdp_*, ...)\n  sources: [well-known/wawanesa-brokerplatform-openid-configuration.json]\n\
  standards:\n- id: csio-api-security-standards\n  name: CSIO API Security Standards\n  status: certified\n  date: '2024-10-29'\n  note: >-\n    \"a standard authentication and authorization API model\" for insurer-to-BMS\n    APIs; certification verifies all security concerns for API endpoints have\n    been addressed\n  source: https://csio.com/news/wawanesa-insurance-achieves-api-security-standards-certification-safeguarding-data-and\nrelated:\n  scopes: scopes/wawanesa-scopes.yml\n  well_known: well-known/wawanesa-well-known.yml\n  conformance: conformance/wawanesa-conformance.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wawanesa/refs/heads/main/authentication/wawanesa-authentication.yml
summary_line: oauth2/openIdConnect · 3 schemes
tags:
- Insurance
- Canada
- Property and Casualty
- Carrier
- Mutual Insurer
- Brokers
- Commercial Lines
- Personal Lines
- Underwriting
- Claims
- Policy Administration
- CSIO
- Partner Gated
---
