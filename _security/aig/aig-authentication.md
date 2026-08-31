---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Aig Authentication
name_suffix: Authentication
oauth_flows: []
overview: AIG declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: AIG
provider_slug: aig
scheme_count: 3
schemes:
- authorization_endpoint: https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7/v1/authorize
  claims:
  - ver
  - jti
  - iss
  - aud
  - iat
  - exp
  - cid
  - uid
  - scp
  - sub
  device_authorization_endpoint: https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7/v1/device/authorize
  end_session_endpoint: https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7/v1/logout
  grant_types:
  - authorization_code
  - implicit
  - refresh_token
  - password
  - client_credentials
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:openid:params:grant-type:ciba
  id_token_encryption_alg:
  - RSA-OAEP-256
  - RSA-OAEP-384
  - RSA-OAEP-512
  id_token_signing_alg: RS256
  introspection_endpoint: https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7/v1/introspect
  issuer: https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7
  jwks_uri: https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7/v1/keys
  name: OAuth2 / OpenID Connect (Okta)
  pkce:
    code_challenge_methods:
    - S256
    supported: true
  protocol: OpenID Connect 1.0
  registration_endpoint: https://auth1.customerpltfm.aig.com/oauth2/v1/clients
  revocation_endpoint: https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7/v1/revoke
  scopes_ref: scopes/aig-scopes.yml
  source: well-known/aig-oauth-authorization-server.json
  token_endpoint: https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7/v1/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - client_secret_jwt
  - private_key_jwt
  - none
  type: oauth2
  userinfo_endpoint: https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7/v1/userinfo
- issuer: https://auth1.customerpltfm.aig.com
  name: OpenID Connect (AIG Okta org issuer)
  openid_configuration: https://auth1.customerpltfm.aig.com/.well-known/openid-configuration
  scopes:
  - openid
  - email
  - profile
  - address
  - phone
  - offline_access
  - groups
  source: well-known/aig-openid-configuration.json
  type: openIdConnect
- applies_to: https://commercial.api.aig.com
  evidence: 'GET https://commercial.api.aig.com/pmp-gateway/c2a/pmp-ext-gtw-api returned HTTP 400 {"error":"Protect Proxy via okta Service Policy: The message does not contain the Authorization header"} — the gateway names Okta as the policy enforcement point and an Authorization header as the required credential.'
  name: Bearer token at the API gateway
  scheme: bearer
  type: http
slug: aig-authentication
source_filename: aig-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: >-\n  https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7/.well-known/oauth-authorization-server\n  (HTTP 200) and https://auth1.customerpltfm.aig.com/.well-known/openid-configuration (HTTP 200),\n  plus observed 400/403 responses from https://commercial.api.aig.com\nprovider: AIG\nproviderId: aig\nsummary: >-\n  AIG publishes no public developer authentication guide, but its production API gateway and the\n  identity provider in front of it are both reachable anonymously enough to read the auth model.\n  commercial.api.aig.com is fronted by an Okta-backed \"Protect Proxy\" that rejects any request\n  without an Authorization header; tokens are issued by AIG's Okta org at\n  auth1.customerpltfm.aig.com, which serves standard OIDC and RFC 8414 discovery documents.\n  There is no anonymous/self-service registration path — client credentials are provisioned to\n  appointed brokers and producers through AIG, not through\
  \ a developer portal signup.\nschemes:\n  - name: OAuth2 / OpenID Connect (Okta)\n    type: oauth2\n    protocol: OpenID Connect 1.0\n    issuer: https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7\n    authorization_endpoint: https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7/v1/authorize\n    token_endpoint: https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7/v1/token\n    userinfo_endpoint: https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7/v1/userinfo\n    jwks_uri: https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7/v1/keys\n    introspection_endpoint: https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7/v1/introspect\n    revocation_endpoint: https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7/v1/revoke\n    end_session_endpoint: https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7/v1/logout\n    device_authorization_endpoint: https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7/v1/device/authorize\n\
  \    registration_endpoint: https://auth1.customerpltfm.aig.com/oauth2/v1/clients\n    grant_types:\n      - authorization_code\n      - implicit\n      - refresh_token\n      - password\n      - client_credentials\n      - urn:ietf:params:oauth:grant-type:device_code\n      - urn:openid:params:grant-type:ciba\n    token_endpoint_auth_methods:\n      - client_secret_basic\n      - client_secret_post\n      - client_secret_jwt\n      - private_key_jwt\n      - none\n    pkce:\n      supported: true\n      code_challenge_methods:\n        - S256\n    id_token_signing_alg: RS256\n    id_token_encryption_alg:\n      - RSA-OAEP-256\n      - RSA-OAEP-384\n      - RSA-OAEP-512\n    claims:\n      - ver\n      - jti\n      - iss\n      - aud\n      - iat\n      - exp\n      - cid\n      - uid\n      - scp\n      - sub\n    scopes_ref: scopes/aig-scopes.yml\n    source: well-known/aig-oauth-authorization-server.json\n  - name: OpenID Connect (AIG Okta org issuer)\n    type: openIdConnect\n    issuer:\
  \ https://auth1.customerpltfm.aig.com\n    openid_configuration: https://auth1.customerpltfm.aig.com/.well-known/openid-configuration\n    scopes:\n      - openid\n      - email\n      - profile\n      - address\n      - phone\n      - offline_access\n      - groups\n    source: well-known/aig-openid-configuration.json\n  - name: Bearer token at the API gateway\n    type: http\n    scheme: bearer\n    applies_to: https://commercial.api.aig.com\n    evidence: >-\n      GET https://commercial.api.aig.com/pmp-gateway/c2a/pmp-ext-gtw-api returned HTTP 400\n      {\"error\":\"Protect Proxy via okta Service Policy: The message does not contain the\n      Authorization header\"} — the gateway names Okta as the policy enforcement point and an\n      Authorization header as the required credential.\nmfa:\n  enforced: true\n  evidence: >-\n    https://www.aig.com/mfa-authentication is a published page in AIG's sitemap and the Producer\n    Management Portal embeds the Okta Sign-In Widget with MFA/OTP\
  \ grant types advertised by the\n    authorization server.\nonboarding:\n  self_service: false\n  note: >-\n    No public signup or sandbox key issuance was found. API credentials are issued to appointed\n    brokers, producers and clients under distribution/technology agreements; the portal login\n    surfaces are https://www.myaig.com and https://www.producermanagementportal.aig.com.\ndocs: null\ndocs_note: >-\n  AIG's developer portal host (www.developers.aig.com) is indexed by search engines but refused\n  TCP connections on both 443 and 80 at the time of this probe, so no published authentication\n  guide could be read.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aig/refs/heads/main/authentication/aig-authentication.yml
summary_line: 3 schemes
tags:
- Insurance
- Financial-Services
- Property Casualty
- Cyber Insurance
- Enterprise
- Fortune 100
---
