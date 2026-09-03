---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Via Science Authentication
name_suffix: Authentication
oauth_flows: []
overview: Via Science declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Via Science
provider_slug: via-science
scheme_count: 4
schemes:
- description: 'OpenID Connect on the VIA Keycloak realm `qt` (Quantum Transfer). Browser clients use Authorization Code with PKCE (S256); the resulting access token is presented as an HTTP Authorization: Bearer JWT.'
  format: JWT
  in: header
  name: openIdConnect
  openIdConnectUrl: https://auth.solvewithvia.com/auth/realms/qt/.well-known/openid-configuration
  scheme: bearer
  source: well-known/via-science-qt-openid-configuration.json
  type: openIdConnect
- description: OpenID Connect on the VIA Keycloak realm `ztf_demo`, the realm backing the public ZTF demo at https://demo.ztf.solvewithvia.com/ and the published tutorials.
  format: JWT
  in: header
  name: openIdConnect-ztf-demo
  openIdConnectUrl: https://auth.solvewithvia.com/auth/realms/ztf_demo/.well-known/openid-configuration
  scheme: bearer
  source: well-known/via-science-ztf-demo-openid-configuration.json
  type: openIdConnect
- description: 'The discovery document advertises `tls_client_auth` as a client-authentication method and `tls_client_certificate_bound_access_tokens: true` (RFC 8705 certificate-bound access tokens). Available, not required.'
  name: mutualTLS
  source: well-known/via-science-qt-openid-configuration.json
  type: mutualTLS
- description: ZTF step-up authentication. Sensitive operations require an additional digital signature produced by the user's VIA Wallet over WalletConnect v2, verified server-side before the action is allowed. Documented in tutorial-2-step-up-auth and tutorial-2-owasp-prompt-injection, whose backend ships both a jwtAuth and a signatureAuth middleware.
  in: body
  name: wallet-signature-step-up
  note: This is VIA's stated defence against an AI agent acting on a user's behalf without explicit consent — the bearer token alone is not sufficient for a sensitive call.
  source: https://github.com/viascience/ztf-tutorial/tree/master/tutorial-2-step-up-auth
  type: signature
slug: via-science-authentication
source_filename: via-science-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: >-\n  https://auth.solvewithvia.com/auth/realms/qt/.well-known/openid-configuration (HTTP 200)\n  and https://auth.solvewithvia.com/auth/realms/ztf_demo/.well-known/openid-configuration\n  (HTTP 200), fetched anonymously 2026-09-02; corroborated by the VIA ZTF integration guide\n  at https://documentation.ztf.solvewithvia.com/integration/ and the tutorial sources at\n  https://github.com/viascience/ztf-tutorial.\nname: VIA (Via Science, Inc.) — authentication profile\ndocs: https://documentation.ztf.solvewithvia.com/integration/\n\nsummary: >-\n  VIA does not publish an API-key surface. Every VIA product surface — the Quantum Transfer\n  (QT) application, the ZTF demo, and any application a customer integrates with VIA Zero\n  Trust Fabric — authenticates through a VIA-operated Keycloak identity server at\n  auth.solvewithvia.com using OpenID Connect Authorization Code + PKCE. The discovery\n  document is served anonymously per\
  \ realm, so the full endpoint set, signing algorithms,\n  grant types and client-authentication methods are machine-readable without credentials.\n  ZTF layers decentralized identity on top: passwordless login backed by W3C Verifiable\n  Credentials held in the VIA Wallet, with wallet-signature step-up for sensitive actions.\n\nschemes:\n  - name: openIdConnect\n    type: openIdConnect\n    in: header\n    scheme: bearer\n    format: JWT\n    openIdConnectUrl: https://auth.solvewithvia.com/auth/realms/qt/.well-known/openid-configuration\n    description: >-\n      OpenID Connect on the VIA Keycloak realm `qt` (Quantum Transfer). Browser clients use\n      Authorization Code with PKCE (S256); the resulting access token is presented as an\n      HTTP Authorization: Bearer JWT.\n    source: well-known/via-science-qt-openid-configuration.json\n\n  - name: openIdConnect-ztf-demo\n    type: openIdConnect\n    in: header\n    scheme: bearer\n    format: JWT\n    openIdConnectUrl: https://auth.solvewithvia.com/auth/realms/ztf_demo/.well-known/openid-configuration\n\
  \    description: >-\n      OpenID Connect on the VIA Keycloak realm `ztf_demo`, the realm backing the public ZTF\n      demo at https://demo.ztf.solvewithvia.com/ and the published tutorials.\n    source: well-known/via-science-ztf-demo-openid-configuration.json\n\n  - name: mutualTLS\n    type: mutualTLS\n    description: >-\n      The discovery document advertises `tls_client_auth` as a client-authentication method\n      and `tls_client_certificate_bound_access_tokens: true` (RFC 8705 certificate-bound\n      access tokens). Available, not required.\n    source: well-known/via-science-qt-openid-configuration.json\n\n  - name: wallet-signature-step-up\n    type: signature\n    in: body\n    description: >-\n      ZTF step-up authentication. Sensitive operations require an additional digital\n      signature produced by the user's VIA Wallet over WalletConnect v2, verified\n      server-side before the action is allowed. Documented in tutorial-2-step-up-auth and\n      tutorial-2-owasp-prompt-injection,\
  \ whose backend ships both a jwtAuth and a\n      signatureAuth middleware.\n    source: https://github.com/viascience/ztf-tutorial/tree/master/tutorial-2-step-up-auth\n    note: >-\n      This is VIA's stated defence against an AI agent acting on a user's behalf without\n      explicit consent — the bearer token alone is not sufficient for a sensitive call.\n\nendpoints:\n  qt:\n    issuer: https://auth.solvewithvia.com/auth/realms/qt\n    authorization: https://auth.solvewithvia.com/auth/realms/qt/protocol/openid-connect/auth\n    token: https://auth.solvewithvia.com/auth/realms/qt/protocol/openid-connect/token\n    userinfo: https://auth.solvewithvia.com/auth/realms/qt/protocol/openid-connect/userinfo\n    jwks: https://auth.solvewithvia.com/auth/realms/qt/protocol/openid-connect/certs\n    end_session: https://auth.solvewithvia.com/auth/realms/qt/protocol/openid-connect/logout\n    introspection: https://auth.solvewithvia.com/auth/realms/qt/protocol/openid-connect/token/introspect\n\
  \    revocation: https://auth.solvewithvia.com/auth/realms/qt/protocol/openid-connect/revoke\n    registration: https://auth.solvewithvia.com/auth/realms/qt/clients-registrations/openid-connect\n    device_authorization: https://auth.solvewithvia.com/auth/realms/qt/protocol/openid-connect/auth/device\n    pushed_authorization_request: https://auth.solvewithvia.com/auth/realms/qt/protocol/openid-connect/ext/par/request\n    backchannel_authentication: https://auth.solvewithvia.com/auth/realms/qt/protocol/openid-connect/ext/ciba/auth\n  ztf_demo:\n    issuer: https://auth.solvewithvia.com/auth/realms/ztf_demo\n    authorization: https://auth.solvewithvia.com/auth/realms/ztf_demo/protocol/openid-connect/auth\n    token: https://auth.solvewithvia.com/auth/realms/ztf_demo/protocol/openid-connect/token\n    userinfo: https://auth.solvewithvia.com/auth/realms/ztf_demo/protocol/openid-connect/userinfo\n    jwks: https://auth.solvewithvia.com/auth/realms/ztf_demo/protocol/openid-connect/certs\n\
  \    end_session: https://auth.solvewithvia.com/auth/realms/ztf_demo/protocol/openid-connect/logout\n    uma2_resource_registration: https://auth.solvewithvia.com/auth/realms/ztf_demo/authz/protection/resource_set\n    uma2_permission: https://auth.solvewithvia.com/auth/realms/ztf_demo/authz/protection/permission\n    uma2_policy: https://auth.solvewithvia.com/auth/realms/ztf_demo/authz/protection/uma-policy\n\ngrant_types_supported:\n  - authorization_code\n  - client_credentials\n  - implicit\n  - password\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:uma-ticket\n  - urn:openid:params:grant-type:ciba\n\nclient_authentication_methods:\n  - private_key_jwt\n  - client_secret_basic\n  - client_secret_post\n  - tls_client_auth\n  - client_secret_jwt\n\ntoken_format: JWT\nid_token_signing_algs:\n  - RS256\n  - RS384\n  - RS512\n\
  \  - PS256\n  - PS384\n  - PS512\n  - ES256\n  - ES384\n  - ES512\n  - EdDSA\n  - HS256\n  - HS384\n  - HS512\n\nfeatures:\n  pkce: true\n  pkce_methods: [plain, S256]\n  dpop: true\n  pushed_authorization_requests: true\n  par_required: false\n  dynamic_client_registration: true\n  device_authorization_grant: true\n  ciba: true\n  token_exchange: true\n  uma2: true\n  mtls_bound_access_tokens: true\n  front_channel_logout: true\n  back_channel_logout: true\n  request_object: true\n  claims_parameter: true\n\nclaims_supported:\n  [iss, sub, aud, exp, iat, auth_time, name, given_name, family_name,\n   preferred_username, email, acr, azp, nonce]\n\nacr_values_supported: ['0', '1']\n\napi_keys:\n  supported: false\n  note: >-\n    No API-key issuance is documented on any public VIA surface. Machine-to-machine access\n    would use the OIDC `client_credentials` grant advertised by the realms above; client\n    provisioning is not self-serve — it goes through the \"Get a demo\" form.\n\ngaps:\n\
  \  - >-\n    No OpenAPI or other machine-readable REST contract is published for any VIA product,\n    so the securitySchemes above are recorded from the OIDC discovery documents and the\n    integration guide rather than derived from a spec.\n  - >-\n    No public self-serve signup: realm clients are provisioned by VIA. The auth surface is\n    fully readable anonymously; the resource APIs behind it are not.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/via-science/refs/heads/main/authentication/via-science-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Security
- Identity
- Authentication
- Zero Trust
- Decentralized Identity
- Verifiable Credentials
- Post-Quantum Cryptography
- Encryption
- File Transfer
- Defense
- Artificial Intelligence
- Blockchain
- OpenID Connect
---
