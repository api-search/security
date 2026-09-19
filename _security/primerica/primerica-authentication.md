---
anonymous_access: false
api_key_in: []
auth_types: []
description: Primerica publishes no developer-facing API and no authentication documentation for third parties. It does, however, serve real anonymous OAuth 2.0 / OpenID Connect provider metadata for the identity systems behind its own first-party applications, and the MyPrimerica client portal ships its runtime OAuth client configuration as a public JavaScript file. This profile is derived entirely from those published discovery documents — it describes how Primerica's own apps authenticate, NOT a partner or public API programme, which does not exist.
kind: authentication
layout: security
mechanism_count: 3
method: probed
name: Primerica Authentication
name_suffix: Authentication
oauth_flows: []
overview: Primerica declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Primerica
provider_slug: primerica
scheme_count: 3
schemes:
- applies_to: first-party Primerica applications only
  name: OpenID Connect
  openIdConnectUrl: https://login.my.primerica.com/oauth2/aus8qhl8ufh9Bx3Dn697/.well-known/openid-configuration
  type: openIdConnect
- applies_to: MyPrimerica client portal SPA
  flows:
    authorizationCode:
      authorizationUrl: https://login.my.primerica.com/oauth2/aus8qhl8ufh9Bx3Dn697/v1/authorize
      refreshUrl: https://login.my.primerica.com/oauth2/aus8qhl8ufh9Bx3Dn697/v1/token
      tokenUrl: https://login.my.primerica.com/oauth2/aus8qhl8ufh9Bx3Dn697/v1/token
  name: OAuth 2.0 authorization code with PKCE
  type: oauth2
- applies_to: gtw.primericaonline.com gateway OAuth provider
  name: mTLS client authentication with certificate-bound access tokens
  type: mutualTLS
slug: primerica-authentication
source_filename: primerica-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: >-\n  https://login.my.primerica.com/oauth2/aus8qhl8ufh9Bx3Dn697/.well-known/openid-configuration,\n  https://login.my.primerica.com/.well-known/openid-configuration,\n  https://login.primericaonline.com/.well-known/openid-configuration,\n  https://gtw.primericaonline.com/.well-known/openid-configuration,\n  https://gtw.primericaonline.com/prod/exp/client/login-bff/v1/oidc/.well-known/openid-configuration,\n  https://www.primerica.com/public/primerica-client-portals.html\nspecification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: Primerica\nproviderId: primerica\ndescription: >-\n  Primerica publishes no developer-facing API and no authentication documentation for third parties.\n  It does, however, serve real anonymous OAuth 2.0 / OpenID Connect provider metadata for the identity\n  systems behind its own first-party applications, and the MyPrimerica client portal ships its runtime\n  OAuth client configuration\
  \ as a public JavaScript file. This profile is derived entirely from those\n  published discovery documents — it describes how Primerica's own apps authenticate, NOT a partner or\n  public API programme, which does not exist.\nnotes: >-\n  Nothing here is a credential and nothing here is obtainable by a third party. There is no public\n  client registration, no developer signup, and no published partner onboarding path. Dynamic client\n  registration endpoints are advertised in the metadata but are Okta/Layer7 platform defaults, not an\n  open registration offer.\nauthorization_servers:\n  - id: myprimerica-client-portal\n    name: MyPrimerica client portal authorization server\n    issuer: https://login.my.primerica.com/oauth2/aus8qhl8ufh9Bx3Dn697\n    platform: Okta (custom domain login.my.primerica.com -> myprimerica.customdomains.okta.com)\n    discovery: https://login.my.primerica.com/oauth2/aus8qhl8ufh9Bx3Dn697/.well-known/openid-configuration\n    artifact: well-known/primerica-login-my-clientportal-openid-configuration.json\n\
  \    serves: https://my.primerica.com/app/v1/ (MyPrimerica policy, investment and account portal)\n    authorization_endpoint: https://login.my.primerica.com/oauth2/aus8qhl8ufh9Bx3Dn697/v1/authorize\n    token_endpoint: https://login.my.primerica.com/oauth2/aus8qhl8ufh9Bx3Dn697/v1/token\n    introspection_endpoint: https://login.my.primerica.com/oauth2/aus8qhl8ufh9Bx3Dn697/v1/introspect\n    revocation_endpoint: https://login.my.primerica.com/oauth2/aus8qhl8ufh9Bx3Dn697/v1/revoke\n    end_session_endpoint: https://login.my.primerica.com/oauth2/aus8qhl8ufh9Bx3Dn697/v1/logout\n    jwks_uri: https://login.my.primerica.com/oauth2/aus8qhl8ufh9Bx3Dn697/v1/keys\n    device_authorization_endpoint: https://login.my.primerica.com/oauth2/aus8qhl8ufh9Bx3Dn697/v1/device/authorize\n    grant_types_supported:\n      - authorization_code\n      - implicit\n      - refresh_token\n      - password\n      - urn:ietf:params:oauth:grant-type:device_code\n      - urn:openid:params:grant-type:ciba\n    pkce:\n\
  \      supported: true\n      code_challenge_methods: [S256]\n    dpop_signing_alg_values_supported: [RS256, RS384, RS512, ES256, ES384, ES512]\n    token_endpoint_auth_methods_supported:\n      - client_secret_basic\n      - client_secret_post\n      - client_secret_jwt\n      - private_key_jwt\n      - none\n    observed_public_client:\n      client_id: 0oa8qisqnhShOMbhR697\n      note: >-\n        Public (PKCE, no secret) SPA client id published by Primerica in its own client-portal\n        directory page and in the MyPrimerica runtime config. Not a credential.\n      requested_scope: openid profile email offline_access client-portal:write cm.readonly\n  - id: okta-org-myprimerica\n    name: MyPrimerica Okta org authorization server\n    issuer: https://login.my.primerica.com\n    platform: Okta\n    discovery: https://login.my.primerica.com/.well-known/openid-configuration\n    artifact: well-known/primerica-login-my-openid-configuration.json\n    scopes_supported: [openid, email,\
  \ profile, address, phone, offline_access, groups]\n    pkce:\n      supported: true\n      code_challenge_methods: [S256]\n  - id: okta-org-pol\n    name: Primerica Online (representative portal) Okta org authorization server\n    issuer: https://login.primericaonline.com\n    platform: Okta (custom domain -> primericaonline.customdomains.okta.com)\n    discovery: https://login.primericaonline.com/.well-known/openid-configuration\n    artifact: well-known/primerica-login-pol-openid-configuration.json\n    serves: >-\n      https://www.primericaonline.com/ — the POL representative portal, which SAML-redirects into this\n      org (SAMLRequest to /app/primericaonline_polapp_1/.../sso/saml)\n    federation: SAML 2.0 SSO in addition to OIDC\n  - id: layer7-gateway\n    name: Primerica API gateway OAuth/OIDC provider\n    issuer: https://gtw.primericaonline.com\n    platform: Broadcom / CA Layer7 API Gateway\n    discovery: https://gtw.primericaonline.com/.well-known/openid-configuration\n\
  \    artifact: well-known/primerica-gtw-openid-configuration.json\n    authorization_endpoint: https://gtw.primericaonline.com:8443/auth/oauth/v2/authorize\n    token_endpoint: https://gtw.primericaonline.com:8443/auth/oauth/v2/token\n    pushed_authorization_request_endpoint: https://gtw.primericaonline.com:8443/auth/oauth/v2/par\n    backchannel_authentication_endpoint: https://gtw.primericaonline.com:8443/auth/oauth/v2/bc-authorize\n    jwks_uri: https://gtw.primericaonline.com:8443/openid/connect/jwks.json\n    scopes_supported: [openid, email, profile, openid_client_registration]\n    grant_types_supported:\n      - authorization_code\n      - implicit\n      - refresh_token\n      - password\n      - client_credentials\n      - urn:ietf:params:oauth:grant-type:jwt-bearer\n      - urn:ietf:params:oauth:grant-type:saml2-bearer\n      - urn:ietf:params:oauth:grant-type:token-exchange\n      - urn:ietf:params:oauth:grant-type:device_code\n      - urn:openid:params:grant-type:ciba\n \
  \   token_endpoint_auth_methods_supported:\n      - client_secret_basic\n      - client_secret_post\n      - client_secret_jwt\n      - private_key_jwt\n      - tls_client_auth\n      - self_signed_tls_client_auth\n    mtls:\n      supported: true\n      certificate_bound_access_tokens: true\n    service_documentation:\n      url: https://gtw.primericaonline.com:8443/apidocs/auth/oauth/v2/swagger\n      status: unreachable\n      note: >-\n        Primerica's own OIDC metadata advertises a Swagger document for the gateway OAuth service, but\n        port 8443 does not accept connections from the public internet (probe 2026-09-14 timed out).\n        The one API description Primerica points at is therefore not publicly retrievable. This is the\n        single highest-value thing the provider could change: exposing that Swagger, or publishing it\n        on 443, would give the gateway a real machine-readable contract.\n  - id: layer7-login-bff\n    name: Client login BFF OIDC provider\n\
  \    issuer: https://gtw.primericaonline.com/prod/exp/client/login-bff/v1/oidc\n    platform: Broadcom / CA Layer7 API Gateway (backend-for-frontend)\n    discovery: https://gtw.primericaonline.com/prod/exp/client/login-bff/v1/oidc/.well-known/openid-configuration\n    artifact: well-known/primerica-gtw-login-bff-openid-configuration.json\n    scopes_supported: [openid, email, profile]\n    grant_types_supported: [authorization_code, implicit, refresh_token]\n    claims_supported: [sub, lastLogin, dcGroups, name, title, userid, email]\nschemes:\n  - type: openIdConnect\n    name: OpenID Connect\n    applies_to: first-party Primerica applications only\n    openIdConnectUrl: https://login.my.primerica.com/oauth2/aus8qhl8ufh9Bx3Dn697/.well-known/openid-configuration\n  - type: oauth2\n    name: OAuth 2.0 authorization code with PKCE\n    applies_to: MyPrimerica client portal SPA\n    flows:\n      authorizationCode:\n        authorizationUrl: https://login.my.primerica.com/oauth2/aus8qhl8ufh9Bx3Dn697/v1/authorize\n\
  \        tokenUrl: https://login.my.primerica.com/oauth2/aus8qhl8ufh9Bx3Dn697/v1/token\n        refreshUrl: https://login.my.primerica.com/oauth2/aus8qhl8ufh9Bx3Dn697/v1/token\n  - type: mutualTLS\n    name: mTLS client authentication with certificate-bound access tokens\n    applies_to: gtw.primericaonline.com gateway OAuth provider\nthird_party_access:\n  public_api: false\n  self_service_signup: false\n  documented_partner_onboarding: false\n  note: >-\n    No public or partner API programme is documented anywhere on Primerica's public surface. Every\n    endpoint above exists to authenticate Primerica's own customers and representatives.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/primerica/refs/heads/main/authentication/primerica-authentication.yml
summary_line: 3 schemes
tags:
- Insurance
- Financial-Services
- Life Insurance
- Identity
- Authentication
- OpenID Connect
- API Gateway
---
