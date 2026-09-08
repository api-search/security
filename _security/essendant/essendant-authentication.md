---
anonymous_access: false
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Essendant Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- implicit
- password
- deviceCode
- jwtBearer
- refreshToken
overview: Essendant secures its APIs with openIdConnect and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, implicit, password, deviceCode, jwtBearer, and refreshToken flow(s).
provider_name: Essendant
provider_slug: essendant
scheme_count: 2
schemes:
- authorization_endpoint: https://sso.essendant.com/adfs/oauth2/authorize/
  device_authorization_endpoint: https://sso.essendant.com/adfs/oauth2/devicecode
  end_session_endpoint: https://sso.essendant.com/adfs/oauth2/logout
  frontchannel_logout_supported: true
  grant_types_supported:
  - authorization_code
  - refresh_token
  - client_credentials
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  - implicit
  - password
  - srv_challenge
  - urn:ietf:params:oauth:grant-type:device_code
  - device_code
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://sso.essendant.com/adfs
  jwks_uri: https://sso.essendant.com/adfs/discovery/keys
  name: essendant-adfs-sso
  openIdConnectUrl: https://sso.essendant.com/adfs/.well-known/openid-configuration
  response_types_supported:
  - code
  - id_token
  - code id_token
  - id_token token
  - code token
  - code id_token token
  sources:
  - well-known/essendant-sso-openid-configuration.json
  subject_types_supported:
  - pairwise
  token_endpoint: https://sso.essendant.com/adfs/oauth2/token/
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  - windows_client_authentication
  type: openIdConnect
  userinfo_endpoint: https://sso.essendant.com/adfs/userinfo
- authorization_endpoint: https://login.essendant.com/adfs/oauth2/authorize/
  device_authorization_endpoint: https://login.essendant.com/adfs/oauth2/devicecode
  end_session_endpoint: https://login.essendant.com/adfs/oauth2/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - client_credentials
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  - implicit
  - password
  - srv_challenge
  - urn:ietf:params:oauth:grant-type:device_code
  - device_code
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://login.essendant.com/adfs
  jwks_uri: https://login.essendant.com/adfs/discovery/keys
  name: essendant-adfs-login
  openIdConnectUrl: https://login.essendant.com/adfs/.well-known/openid-configuration
  sources:
  - well-known/essendant-login-openid-configuration.json
  token_endpoint: https://login.essendant.com/adfs/oauth2/token/
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  - windows_client_authentication
  type: openIdConnect
  userinfo_endpoint: https://login.essendant.com/adfs/userinfo
slug: essendant-authentication
source_filename: essendant-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: https://sso.essendant.com/adfs/.well-known/openid-configuration\nscope_note: >-\n  Essendant publishes no public API and therefore no API authentication reference. What it\n  DOES publish, anonymously and in machine-readable form, is OpenID Connect discovery\n  metadata for the Active Directory Federation Services deployment that fronts its\n  reseller and customer portals (Solutions Central, Azerty, BiggestBook, Empower Central).\n  This file records that identity surface exactly as fetched. It is portal SSO, not an API\n  authorization server: there is no dynamic client registration, no published client\n  onboarding, and no resource server documented against it. Do not read this artifact as\n  evidence of a developer program.\nsummary:\n  types: [openIdConnect, oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, clientCredentials, implicit, password, deviceCode, jwtBearer, refreshToken]\n  mutual_tls: false\n  dynamic_client_registration:\
  \ false\n  protected_resource_metadata: false\nschemes:\n- name: essendant-adfs-sso\n  type: openIdConnect\n  openIdConnectUrl: https://sso.essendant.com/adfs/.well-known/openid-configuration\n  issuer: https://sso.essendant.com/adfs\n  authorization_endpoint: https://sso.essendant.com/adfs/oauth2/authorize/\n  token_endpoint: https://sso.essendant.com/adfs/oauth2/token/\n  userinfo_endpoint: https://sso.essendant.com/adfs/userinfo\n  device_authorization_endpoint: https://sso.essendant.com/adfs/oauth2/devicecode\n  end_session_endpoint: https://sso.essendant.com/adfs/oauth2/logout\n  jwks_uri: https://sso.essendant.com/adfs/discovery/keys\n  token_endpoint_auth_methods_supported: [client_secret_post, client_secret_basic, private_key_jwt, windows_client_authentication]\n  response_types_supported: [code, id_token, code id_token, id_token token, code token, code id_token token]\n  grant_types_supported: [authorization_code, refresh_token, client_credentials, 'urn:ietf:params:oauth:grant-type:jwt-bearer',\
  \ implicit, password, srv_challenge, 'urn:ietf:params:oauth:grant-type:device_code', device_code]\n  id_token_signing_alg_values_supported: [RS256]\n  subject_types_supported: [pairwise]\n  frontchannel_logout_supported: true\n  sources: [well-known/essendant-sso-openid-configuration.json]\n- name: essendant-adfs-login\n  type: openIdConnect\n  openIdConnectUrl: https://login.essendant.com/adfs/.well-known/openid-configuration\n  issuer: https://login.essendant.com/adfs\n  authorization_endpoint: https://login.essendant.com/adfs/oauth2/authorize/\n  token_endpoint: https://login.essendant.com/adfs/oauth2/token/\n  userinfo_endpoint: https://login.essendant.com/adfs/userinfo\n  device_authorization_endpoint: https://login.essendant.com/adfs/oauth2/devicecode\n  end_session_endpoint: https://login.essendant.com/adfs/oauth2/logout\n  jwks_uri: https://login.essendant.com/adfs/discovery/keys\n  token_endpoint_auth_methods_supported: [client_secret_post, client_secret_basic, private_key_jwt,\
  \ windows_client_authentication]\n  grant_types_supported: [authorization_code, refresh_token, client_credentials, 'urn:ietf:params:oauth:grant-type:jwt-bearer', implicit, password, srv_challenge, 'urn:ietf:params:oauth:grant-type:device_code', device_code]\n  id_token_signing_alg_values_supported: [RS256]\n  sources: [well-known/essendant-login-openid-configuration.json]\nfederation:\n- protocol: WS-Trust / WS-Federation\n  metadata: https://sso.essendant.com/adfs/services/trust/mex\n  http_status: 200\n  format: WSDL 1.1 (WS-MetadataExchange)\n  bytes: 26665\n  note: >-\n    Fetched and confirmed to parse as WSDL, but it is Microsoft's stock AD FS Security\n    Token Service contract — targetNamespace\n    http://schemas.microsoft.com/ws/2008/06/identity/securitytokenservice — not an API\n    Essendant authored. Recorded as identity evidence only. Deliberately NOT registered as\n    a WSDL contract in apis.yml: crediting a vendor-default STS endpoint as a published\n    SOAP API would\
  \ be a false positive on contract_present.\n- protocol: SAML 2.0\n  metadata: https://sso.essendant.com/FederationMetadata/2007-06/FederationMetadata.xml\n  http_status: 200\n  entity_id: http://sso.essendant.com/adfs/services/trust\n  bytes: 82481\n- protocol: SAML 2.0\n  metadata: https://login.essendant.com/FederationMetadata/2007-06/FederationMetadata.xml\n  http_status: 200\n  entity_id: http://login.essendant.com/adfs/services/trust\n  bytes: 81680\ndocs: null\ndocs_note: >-\n  No public authentication documentation was found. Access to Essendant's portals and to\n  the ECDB product-content feed is arranged through an account manager; Essendant directs\n  integrators to TechSupport@Essendant.com rather than to a developer reference.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/essendant/refs/heads/main/authentication/essendant-authentication.yml
summary_line: openIdConnect/oauth2 · 2 schemes
tags:
- Wholesale
- Distribution
- Supply Chain
- Office Supplies
- Fulfillment
- 3PL
- B2B
- EDI
- Ecommerce
- JanSan
- Foodservice
---
