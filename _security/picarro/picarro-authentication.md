---
api_key_in: []
api_specs:
- filename: picarro-sam-foup-asyncapi.yml
  format: yaml
  label: Picarro Edge — SAM FOUP gRPC API
  slug: picarro-edge-sam-foup-grpc-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/picarro/refs/heads/main/asyncapi/picarro-sam-foup-asyncapi.yml
auth_types:
- openIdConnect
- oauth2
- saml2
- none
description: ''
kind: authentication
layout: security
method: probed
name: Picarro Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- password
- clientCredentials
- refreshToken
overview: Picarro secures its APIs with openIdConnect, oauth2, saml2, and none across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, password, clientCredentials, and refreshToken flow(s).
provider_name: Picarro
provider_slug: picarro
scheme_count: 3
schemes:
- backchannel_logout: true
  claims:
  - aud
  - sub
  - iss
  - auth_time
  - name
  - given_name
  - family_name
  - preferred_username
  - email
  - acr
  endpoints:
    authorization: https://identity-prod.picarro.com/auth/realms/picarro/protocol/openid-connect/auth
    dynamic_registration: https://identity-prod.picarro.com/auth/realms/picarro/clients-registrations/openid-connect
    end_session: https://identity-prod.picarro.com/auth/realms/picarro/protocol/openid-connect/logout
    introspection: https://identity-prod.picarro.com/auth/realms/picarro/protocol/openid-connect/token/introspect
    jwks: https://identity-prod.picarro.com/auth/realms/picarro/protocol/openid-connect/certs
    revocation: https://identity-prod.picarro.com/auth/realms/picarro/protocol/openid-connect/revoke
    token: https://identity-prod.picarro.com/auth/realms/picarro/protocol/openid-connect/token
    userinfo: https://identity-prod.picarro.com/auth/realms/picarro/protocol/openid-connect/userinfo
  grant_types:
  - authorization_code
  - implicit
  - refresh_token
  - password
  - client_credentials
  id_token_signing_algs:
  - RS256
  - RS384
  - RS512
  - PS256
  - PS384
  - PS512
  - ES256
  - ES384
  - ES512
  - HS256
  - HS384
  - HS512
  implementation: Keycloak (realm "picarro")
  issuer: https://identity-prod.picarro.com/auth/realms/picarro
  mtls_bound_tokens: true
  name: PicarroIdentityOIDC
  openIdConnectUrl: https://identity-prod.picarro.com/auth/realms/picarro/.well-known/openid-configuration
  pkce:
  - S256
  - plain
  scopes:
  - openid
  - email
  - address
  - phone
  - roles
  - web-origins
  - microprofile-jwt
  - offline_access
  - profile
  sources:
  - well-known/picarro-openid-configuration.json
  token_endpoint_auth_methods:
  - private_key_jwt
  - client_secret_basic
  - client_secret_post
  - tls_client_auth
  - client_secret_jwt
  type: openIdConnect
- description: The P-Cubed web application (https://pcubed.picarro.com/) redirects unauthenticated browsers to the same Keycloak realm over SAML 2.0 (/protocol/saml?SAMLRequest=...), observed on an anonymous GET of the portal root.
  endpoint: https://identity-prod.picarro.com/auth/realms/picarro/protocol/saml
  name: PicarroSAMLSSO
  sources:
  - probe https://pcubed.picarro.com/
  type: saml2
- description: The on-premise Picarro Edge gRPC server (picarro-edge, TCP 3343) and Platform Server (platformserver, TCP 7528) accept plaintext ("insecure") gRPC client connections by default, per the first-party README. No transport security or per-call credential is documented for these edge services; they are intended to run on a customer-controlled instrument network.
  name: PicarroEdgeGRPC
  ports:
  - 3343
  - 7528
  reflection: true
  sources:
  - https://github.com/picarro/sam-foup-public
  transport: grpc (h2c, plaintext)
  type: none
slug: picarro-authentication
source_filename: picarro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: https://identity-prod.picarro.com/auth/realms/picarro/.well-known/openid-configuration\ndocs: https://github.com/picarro/sam-foup-public\nnotes: >-\n  Picarro publishes no OpenAPI, so this profile is not derived from securitySchemes.\n  It is assembled from two real, fetched sources: the anonymous Keycloak OIDC discovery\n  document that fronts the P-Cubed cloud platform, and the first-party gRPC interface\n  README for the on-premise Picarro Edge / Platform Server services.\nsummary:\n  types: [openIdConnect, oauth2, saml2, none]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, implicit, password, clientCredentials, refreshToken]\nschemes:\n  - name: PicarroIdentityOIDC\n    type: openIdConnect\n    openIdConnectUrl: https://identity-prod.picarro.com/auth/realms/picarro/.well-known/openid-configuration\n    issuer: https://identity-prod.picarro.com/auth/realms/picarro\n    implementation: Keycloak (realm \"picarro\")\n\
  \    endpoints:\n      authorization: https://identity-prod.picarro.com/auth/realms/picarro/protocol/openid-connect/auth\n      token: https://identity-prod.picarro.com/auth/realms/picarro/protocol/openid-connect/token\n      userinfo: https://identity-prod.picarro.com/auth/realms/picarro/protocol/openid-connect/userinfo\n      introspection: https://identity-prod.picarro.com/auth/realms/picarro/protocol/openid-connect/token/introspect\n      revocation: https://identity-prod.picarro.com/auth/realms/picarro/protocol/openid-connect/revoke\n      end_session: https://identity-prod.picarro.com/auth/realms/picarro/protocol/openid-connect/logout\n      jwks: https://identity-prod.picarro.com/auth/realms/picarro/protocol/openid-connect/certs\n      dynamic_registration: https://identity-prod.picarro.com/auth/realms/picarro/clients-registrations/openid-connect\n    grant_types: [authorization_code, implicit, refresh_token, password, client_credentials]\n    pkce: [S256, plain]\n    token_endpoint_auth_methods:\
  \ [private_key_jwt, client_secret_basic, client_secret_post, tls_client_auth, client_secret_jwt]\n    mtls_bound_tokens: true\n    backchannel_logout: true\n    id_token_signing_algs: [RS256, RS384, RS512, PS256, PS384, PS512, ES256, ES384, ES512, HS256, HS384, HS512]\n    scopes: [openid, email, address, phone, roles, web-origins, microprofile-jwt, offline_access, profile]\n    claims: [aud, sub, iss, auth_time, name, given_name, family_name, preferred_username, email, acr]\n    sources: [well-known/picarro-openid-configuration.json]\n  - name: PicarroSAMLSSO\n    type: saml2\n    description: >-\n      The P-Cubed web application (https://pcubed.picarro.com/) redirects unauthenticated\n      browsers to the same Keycloak realm over SAML 2.0 (/protocol/saml?SAMLRequest=...),\n      observed on an anonymous GET of the portal root.\n    endpoint: https://identity-prod.picarro.com/auth/realms/picarro/protocol/saml\n    sources: [probe https://pcubed.picarro.com/]\n  - name: PicarroEdgeGRPC\n\
  \    type: none\n    description: >-\n      The on-premise Picarro Edge gRPC server (picarro-edge, TCP 3343) and Platform Server\n      (platformserver, TCP 7528) accept plaintext (\"insecure\") gRPC client connections by\n      default, per the first-party README. No transport security or per-call credential is\n      documented for these edge services; they are intended to run on a customer-controlled\n      instrument network.\n    transport: grpc (h2c, plaintext)\n    ports: [3343, 7528]\n    reflection: true\n    sources: [https://github.com/picarro/sam-foup-public]\nx-evidence:\n  - {url: 'https://identity-prod.picarro.com/auth/realms/picarro/.well-known/openid-configuration', http_status: 200, content_type: application/json, fetched: '2026-08-02'}\n  - {url: 'https://pcubed.picarro.com/', http_status: 200, note: '302 chain to Keycloak SAML endpoint', fetched: '2026-08-02'}\n  - {url: 'https://github.com/picarro/sam-foup-public', http_status: 200, fetched: '2026-08-02'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/picarro/refs/heads/main/authentication/picarro-authentication.yml
summary_line: openIdConnect/oauth2/saml2/none · 3 schemes
tags:
- Company
- Gas Detection
- Environmental Monitoring
- Emissions
- Methane
- Greenhouse Gas
- Scientific Instruments
- Semiconductors
- Industrial IoT
- Sensors
- Analytics
- gRPC
---
