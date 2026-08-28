---
api_key_in: []
auth_types: []
description: OncoLens publishes no public API and no developer authentication documentation. What it does serve, anonymously and on its own domain, is a complete OpenID Connect Discovery document for the identity provider that fronts the customer application. This profile is derived entirely from that document plus the observed sign-in redirect chain — it describes how a human signs in to the OncoLens SaaS, not how a developer would authenticate against a product API, because no product API is published.
kind: authentication
layout: security
method: probed
name: Oncolens Authentication
name_suffix: Authentication
oauth_flows: []
overview: OncoLens declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: OncoLens
provider_slug: oncolens
scheme_count: 0
schemes: []
slug: oncolens-authentication
source_filename: oncolens-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://login.oncolens.com/.well-known/openid-configuration\nname: OncoLens authentication profile\ndescription: >-\n  OncoLens publishes no public API and no developer authentication documentation. What it\n  does serve, anonymously and on its own domain, is a complete OpenID Connect Discovery\n  document for the identity provider that fronts the customer application. This profile is\n  derived entirely from that document plus the observed sign-in redirect chain — it describes\n  how a human signs in to the OncoLens SaaS, not how a developer would authenticate against a\n  product API, because no product API is published.\nscope_of_this_artifact: user-sign-in-only\napi_authentication_documented: false\napi_authentication_note: >-\n  No developer portal, API reference, API key issuance flow, or partner authentication guide\n  exists on any OncoLens host. Access to the platform is through the application UI at\n  signin.oncolens.com.\n\
  identity_provider:\n  issuer: https://login.oncolens.com/\n  platform: Auth0\n  platform_evidence: >-\n    login.oncolens.com is an Auth0 custom domain — DNS CNAME chain resolves through\n    oncolens-prod-cd-a5uiupzhjmdoqgm4.edge.tenants.us.auth0.com and oncolens-prod.us.auth0.com;\n    the discovery document also advertises Auth0-proprietary grant type URNs under\n    http://auth0.com/oauth/grant-type/.\n  tenant_region: us\nsecurity_schemes:\n- key: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://login.oncolens.com/.well-known/openid-configuration\n  description: >-\n    OpenID Connect Discovery 1.0 / RFC 8414. Full authorization-server metadata is served\n    anonymously; the same payload is returned at /.well-known/oauth-authorization-server.\n- key: oauth2\n  type: oauth2\n  description: OAuth 2.0 authorization server backing the OIDC layer.\n  flows:\n    authorizationCode:\n      authorizationUrl: https://login.oncolens.com/authorize\n      tokenUrl: https://login.oncolens.com/oauth/token\n\
  \      refreshUrl: https://login.oncolens.com/oauth/token\n      pkce: required-capable\n      pkce_methods: [S256, plain]\n    clientCredentials:\n      tokenUrl: https://login.oncolens.com/oauth/token\n      note: >-\n        client_credentials is advertised in grant_types_supported. This is the grant a\n        machine-to-machine integration would use — but OncoLens documents no resource\n        API to call with the resulting token.\n    deviceCode:\n      deviceAuthorizationUrl: https://login.oncolens.com/oauth/device/code\n      tokenUrl: https://login.oncolens.com/oauth/token\n      grant: urn:ietf:params:oauth:grant-type:device_code\n    implicit:\n      authorizationUrl: https://login.oncolens.com/authorize\n      note: Advertised but legacy; PKCE authorization_code is the current recommendation.\n- key: saml2\n  type: saml\n  description: >-\n    Enterprise SAML 2.0 SSO observed on secure.oncolens.com, which 302s to\n    login.microsoftonline.com/4338d2c6-1192-445d-be9f-711a3dd11cac/saml2\
  \ with a SAMLRequest —\n    i.e. a Microsoft Entra ID federation for that surface.\n  evidence:\n    url: https://secure.oncolens.com/\n    http_status: 200\n    redirected_to: login.microsoftonline.com (SAML2 endpoint)\nendpoints:\n  authorization: https://login.oncolens.com/authorize\n  token: https://login.oncolens.com/oauth/token\n  userinfo: https://login.oncolens.com/userinfo\n  jwks: https://login.oncolens.com/.well-known/jwks.json\n  revocation: https://login.oncolens.com/oauth/revoke\n  device_authorization: https://login.oncolens.com/oauth/device/code\n  dynamic_client_registration: https://login.oncolens.com/oidc/register\n  backchannel_authentication: https://login.oncolens.com/bc-authorize\n  mfa_challenge: https://login.oncolens.com/mfa/challenge\n  global_token_revocation: https://login.oncolens.com/oauth/global-token-revocation/connection/{connectionName}\ntoken_characteristics:\n  id_token_signing_alg_values_supported: [HS256, RS256, PS256]\n  token_endpoint_auth_methods_supported:\n\
  \  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - none\n  token_endpoint_auth_signing_alg_values_supported: [RS256, RS384, PS256]\n  dpop_signing_alg_values_supported: [ES256]\n  subject_types_supported: [public]\n  response_modes_supported: [query, fragment, form_post]\n  response_types_supported: [code, token, id_token, code token, code id_token, token id_token, code token id_token]\ngrant_types_supported:\n- client_credentials\n- authorization_code\n- refresh_token\n- password\n- implicit\n- urn:ietf:params:oauth:grant-type:device_code\n- urn:ietf:params:oauth:grant-type:token-exchange\n- urn:ietf:params:oauth:grant-type:jwt-bearer\n- http://auth0.com/oauth/grant-type/password-realm\n- http://auth0.com/oauth/grant-type/passwordless/otp\n- http://auth0.com/oauth/grant-type/mfa-oob\n- http://auth0.com/oauth/grant-type/mfa-otp\n- http://auth0.com/oauth/grant-type/mfa-recovery-code\nmfa:\n  supported: true\n  evidence: >-\n    mfa_challenge_endpoint is present,\
  \ and four Auth0 MFA grant types (mfa-oob, mfa-otp,\n    mfa-recovery-code, and the password-realm companion) are advertised.\nsession_management:\n  backchannel_logout_supported: true\n  backchannel_logout_session_supported: true\nobservations:\n- >-\n  Dynamic client registration is advertised at /oidc/register. Whether it is open or gated\n  was NOT tested — this pipeline does not attempt registration against a live production\n  identity provider.\n- >-\n  `none` appears in token_endpoint_auth_methods_supported, which is normal and correct for\n  public/SPA clients using PKCE, and is not on its own a weakness.\n- >-\n  The `password` and `implicit` grants remain enabled. Both are discouraged by OAuth 2.1 /\n  the OAuth Security BCP; this is Auth0 tenant default surface rather than a documented\n  OncoLens choice, and is recorded here as observed configuration only.\nchecked: '2026-08-26'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oncolens/refs/heads/main/authentication/oncolens-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Healthcare
- Oncology
- Cancer Care
- Clinical Trials
- Health Data
- Real World Data
- Artificial Intelligence
- Analytics
- Clinical Workflow
- Cancer Registry
- Life Sciences
- SaaS
---
