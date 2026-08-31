---
api_key_in: []
auth_types: []
description: 'Porsche publishes no public API and no OpenAPI document, so this profile is not derived from a securitySchemes block. It is read directly from the two OpenID Connect discovery documents Porsche serves anonymously: the Porsche ID identity provider at identity.porsche.com and the Porsche CIAM backend-for-frontend fronted by login.porsche.com. These describe how a Porsche Partner Company authenticates once it has been granted access; the APIs themselves stay behind the partner gate.'
kind: authentication
layout: security
method: probed
name: Porsche Authentication
name_suffix: Authentication
oauth_flows: []
overview: Porsche declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Porsche
provider_slug: porsche
scheme_count: 2
schemes:
- ciba:
    delivery_modes:
    - poll
    supported: true
  claims:
  - aud
  - auth_time
  - created_at
  - email
  - email_verified
  - exp
  - family_name
  - given_name
  - iat
  - identities
  - iss
  - name
  - nickname
  - phone_number
  - picture
  - sub
  client_auth_signing_algs:
  - RS256
  - RS384
  - PS256
  client_authentication:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  discovery: https://identity.porsche.com/.well-known/openid-configuration
  dynamic_client_registration: true
  endpoints:
    authorization: https://identity.porsche.com/authorize
    backchannel_authentication: https://identity.porsche.com/bc-authorize
    device_authorization: https://identity.porsche.com/oauth/device/code
    global_token_revocation: https://identity.porsche.com/oauth/global-token-revocation/connection/{connectionName}
    mfa_challenge: https://identity.porsche.com/mfa/challenge
    registration: https://identity.porsche.com/oidc/register
    revocation: https://identity.porsche.com/oauth/revoke
    token: https://identity.porsche.com/oauth/token
    userinfo: https://identity.porsche.com/userinfo
  grant_profiles:
  - urn:ietf:params:oauth:grant-profile:id-jag
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  - implicit
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  - http://auth0.com/oauth/grant-type/password-realm
  - http://auth0.com/oauth/grant-type/passwordless/otp
  - http://auth0.com/oauth/grant-type/mfa-oob
  - http://auth0.com/oauth/grant-type/mfa-otp
  - http://auth0.com/oauth/grant-type/mfa-recovery-code
  id: porsche_id_oidc
  id_token_signing_algs:
  - HS256
  - RS256
  - PS256
  issuer: https://identity.porsche.com/
  jwks_uri: https://identity.porsche.com/.well-known/jwks.json
  logout:
    backchannel_logout: true
    backchannel_logout_session: true
    end_session_endpoint: null
  name: Porsche ID (OpenID Connect)
  note: The discovery document's grant list and the /mfa/challenge endpoint identify this as an Auth0-hosted tenant operating under Porsche's own domain and TLS certificate.
  pkce:
    code_challenge_methods:
    - S256
    - plain
    supported: true
  response_modes:
  - query
  - fragment
  - form_post
  response_types:
  - code
  - token
  - id_token
  - code token
  - code id_token
  - token id_token
  - code token id_token
  sender_constraining:
    dpop: true
    dpop_signing_alg_values:
    - ES256
    mutual_tls: false
  subject_types:
  - public
  type: openIdConnect
- discovery: https://login.porsche.com/.well-known/openid-configuration
  endpoints:
    authorization: https://identity.porsche.com/authorize
    token: https://bff.p-dub.ciamprod.aws.platform.porsche.cloud/api/v2/token
  id: porsche_ciam_bff
  id_token_signing_algs:
  - RS256
  issuer: https://bff.p-dub.ciamprod.aws.platform.porsche.cloud
  jwks_uri: https://bff.p-dub.ciamprod.aws.platform.porsche.cloud/.well-known/jwks.json
  name: Porsche CIAM backend-for-frontend
  note: A thin second discovery document. Authorization is delegated to identity.porsche.com; only the token exchange runs on the CIAM BFF. The issuer sits on platform.porsche.cloud, a Porsche-operated AWS platform domain — different hostname, same company, confirmed by login.porsche.com serving it under Porsche's certificate.
  response_types:
  - id_token
  subject_types:
  - public
  type: openIdConnect
slug: porsche-authentication
source_filename: porsche-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: https://identity.porsche.com/.well-known/openid-configuration\ndocs: https://developer.porsche.com/\nprovider: Porsche\nproviderId: porsche\ndescription: >-\n  Porsche publishes no public API and no OpenAPI document, so this profile is not derived\n  from a securitySchemes block. It is read directly from the two OpenID Connect discovery\n  documents Porsche serves anonymously: the Porsche ID identity provider at\n  identity.porsche.com and the Porsche CIAM backend-for-frontend fronted by\n  login.porsche.com. These describe how a Porsche Partner Company authenticates once it\n  has been granted access; the APIs themselves stay behind the partner gate.\nsummary:\n  primary_scheme: openIdConnect\n  public_registration: false\n  gate: >-\n    Only Porsche AG and approved Porsche Partner Companies may obtain credentials. The\n    Porsche ID Developer Portal FAQ states plainly \"We do not offer any public APIs\".\nschemes:\n  - id:\
  \ porsche_id_oidc\n    type: openIdConnect\n    name: Porsche ID (OpenID Connect)\n    issuer: https://identity.porsche.com/\n    discovery: https://identity.porsche.com/.well-known/openid-configuration\n    jwks_uri: https://identity.porsche.com/.well-known/jwks.json\n    endpoints:\n      authorization: https://identity.porsche.com/authorize\n      token: https://identity.porsche.com/oauth/token\n      userinfo: https://identity.porsche.com/userinfo\n      device_authorization: https://identity.porsche.com/oauth/device/code\n      backchannel_authentication: https://identity.porsche.com/bc-authorize\n      mfa_challenge: https://identity.porsche.com/mfa/challenge\n      revocation: https://identity.porsche.com/oauth/revoke\n      registration: https://identity.porsche.com/oidc/register\n      global_token_revocation: https://identity.porsche.com/oauth/global-token-revocation/connection/{connectionName}\n    grant_types:\n      - authorization_code\n      - client_credentials\n      -\
  \ refresh_token\n      - implicit\n      - password\n      - urn:ietf:params:oauth:grant-type:device_code\n      - urn:ietf:params:oauth:grant-type:token-exchange\n      - urn:ietf:params:oauth:grant-type:jwt-bearer\n      - http://auth0.com/oauth/grant-type/password-realm\n      - http://auth0.com/oauth/grant-type/passwordless/otp\n      - http://auth0.com/oauth/grant-type/mfa-oob\n      - http://auth0.com/oauth/grant-type/mfa-otp\n      - http://auth0.com/oauth/grant-type/mfa-recovery-code\n    response_types:\n      - code\n      - token\n      - id_token\n      - code token\n      - code id_token\n      - token id_token\n      - code token id_token\n    response_modes: [query, fragment, form_post]\n    pkce:\n      supported: true\n      code_challenge_methods: [S256, plain]\n    sender_constraining:\n      dpop: true\n      dpop_signing_alg_values: [ES256]\n      mutual_tls: false\n    client_authentication:\n      - client_secret_basic\n      - client_secret_post\n      - private_key_jwt\n\
  \      - none\n    client_auth_signing_algs: [RS256, RS384, PS256]\n    id_token_signing_algs: [HS256, RS256, PS256]\n    subject_types: [public]\n    dynamic_client_registration: true\n    ciba:\n      supported: true\n      delivery_modes: [poll]\n    logout:\n      backchannel_logout: true\n      backchannel_logout_session: true\n      end_session_endpoint: null\n    grant_profiles:\n      - urn:ietf:params:oauth:grant-profile:id-jag\n    claims:\n      - aud\n      - auth_time\n      - created_at\n      - email\n      - email_verified\n      - exp\n      - family_name\n      - given_name\n      - iat\n      - identities\n      - iss\n      - name\n      - nickname\n      - phone_number\n      - picture\n      - sub\n    note: >-\n      The discovery document's grant list and the /mfa/challenge endpoint identify this as an\n      Auth0-hosted tenant operating under Porsche's own domain and TLS certificate.\n  - id: porsche_ciam_bff\n    type: openIdConnect\n    name: Porsche CIAM backend-for-frontend\n\
  \    issuer: https://bff.p-dub.ciamprod.aws.platform.porsche.cloud\n    discovery: https://login.porsche.com/.well-known/openid-configuration\n    jwks_uri: https://bff.p-dub.ciamprod.aws.platform.porsche.cloud/.well-known/jwks.json\n    endpoints:\n      authorization: https://identity.porsche.com/authorize\n      token: https://bff.p-dub.ciamprod.aws.platform.porsche.cloud/api/v2/token\n    response_types: [id_token]\n    id_token_signing_algs: [RS256]\n    subject_types: [public]\n    note: >-\n      A thin second discovery document. Authorization is delegated to identity.porsche.com;\n      only the token exchange runs on the CIAM BFF. The issuer sits on\n      platform.porsche.cloud, a Porsche-operated AWS platform domain — different hostname,\n      same company, confirmed by login.porsche.com serving it under Porsche's certificate.\nportal_gates:\n  - host: portal.developer.porsche.com\n    mechanism: Microsoft Entra ID (Azure AD) OAuth 2.0 authorization code\n    tenant: 56564e0f-83d3-4b52-92e8-a6bb9ea36564\n\
  \    evidence: >-\n      GET https://portal.developer.porsche.com 302s to\n      login.microsoftonline.com/<tenant>/oauth2/v2.0/authorize with scope \"openid email\".\n    status: 200\n  - host: developerhub.porsche.io\n    mechanism: NextAuth sign-in offering \"Sign in with Entra ID\" and \"Sign in with KUMS MFA\"\n    evidence: GET /docs redirects to /api/auth/signin?callbackUrl=/docs\n    status: 200\nevidence:\n  - url: https://identity.porsche.com/.well-known/openid-configuration\n    status: 200\n  - url: https://login.porsche.com/.well-known/openid-configuration\n    status: 200\n  - url: https://portal.developer.porsche.com\n    status: 200\n  - url: https://developerhub.porsche.io/docs\n    status: 200\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/porsche/refs/heads/main/authentication/porsche-authentication.yml
summary_line: 2 schemes
tags:
- Automobiles
- Cars
- Vehicles
- Automotive
- Connected Car
- Identity
- OpenID Connect
- Design System
- Open Source
- Germany
---
