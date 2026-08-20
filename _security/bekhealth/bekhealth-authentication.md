---
api_key_in: []
auth_types: []
description: BEKhealth publishes no public API and no public authentication documentation. What it does expose anonymously is the OpenID Connect discovery document for its Auth0 custom-domain issuer at auth.bekhealth.com, which is the identity provider guarding both the customer application and the documentation portal at docs.bekhealth.com. This profile is derived entirely from that discovery document — it describes how BEKhealth authenticates users of its platform, not a published API authentication model, because no API contract is public.
kind: authentication
layout: security
method: probed
name: Bekhealth Authentication
name_suffix: Authentication
oauth_flows: []
overview: BEKHealth declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: BEKHealth
provider_slug: bekhealth
scheme_count: 2
schemes:
- description: OpenID Connect 1.0 discovery published by the Auth0 tenant. Authorization Code with PKCE (S256) is supported, alongside client credentials, refresh token, device code, token exchange and JWT bearer grants.
  endpoints:
    authorization: https://auth.bekhealth.com/authorize
    device_authorization: https://auth.bekhealth.com/oauth/device/code
    dynamic_registration: https://auth.bekhealth.com/oidc/register
    jwks: https://auth.bekhealth.com/.well-known/jwks.json
    mfa_challenge: https://auth.bekhealth.com/mfa/challenge
    revocation: https://auth.bekhealth.com/oauth/revoke
    token: https://auth.bekhealth.com/oauth/token
    userinfo: https://auth.bekhealth.com/userinfo
  key: openIdConnect
  openIdConnectUrl: https://auth.bekhealth.com/.well-known/openid-configuration
  type: openIdConnect
- description: OAuth 2.0 authorization-server metadata is served at /.well-known/oauth-authorization-server and is byte-identical in substance to the OIDC discovery document (the Auth0 default). Machine-to-machine access would use the client_credentials grant against the same token endpoint, but no resource server, audience or API scope is published.
  flows:
    authorizationCode:
      authorizationUrl: https://auth.bekhealth.com/authorize
      refreshUrl: https://auth.bekhealth.com/oauth/token
      tokenUrl: https://auth.bekhealth.com/oauth/token
    clientCredentials:
      tokenUrl: https://auth.bekhealth.com/oauth/token
  key: oauth2
  type: oauth2
slug: bekhealth-authentication
source_filename: bekhealth-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: https://auth.bekhealth.com/.well-known/openid-configuration\ndescription: >-\n  BEKhealth publishes no public API and no public authentication documentation.\n  What it does expose anonymously is the OpenID Connect discovery document for\n  its Auth0 custom-domain issuer at auth.bekhealth.com, which is the identity\n  provider guarding both the customer application and the documentation portal\n  at docs.bekhealth.com. This profile is derived entirely from that discovery\n  document — it describes how BEKhealth authenticates users of its platform, not\n  a published API authentication model, because no API contract is public.\nissuer: https://auth.bekhealth.com/\nprovider: Auth0 (custom domain)\nschemes:\n- key: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://auth.bekhealth.com/.well-known/openid-configuration\n  description: >-\n    OpenID Connect 1.0 discovery published by the Auth0 tenant. Authorization\n\
  \    Code with PKCE (S256) is supported, alongside client credentials, refresh\n    token, device code, token exchange and JWT bearer grants.\n  endpoints:\n    authorization: https://auth.bekhealth.com/authorize\n    token: https://auth.bekhealth.com/oauth/token\n    userinfo: https://auth.bekhealth.com/userinfo\n    jwks: https://auth.bekhealth.com/.well-known/jwks.json\n    revocation: https://auth.bekhealth.com/oauth/revoke\n    device_authorization: https://auth.bekhealth.com/oauth/device/code\n    dynamic_registration: https://auth.bekhealth.com/oidc/register\n    mfa_challenge: https://auth.bekhealth.com/mfa/challenge\n- key: oauth2\n  type: oauth2\n  description: >-\n    OAuth 2.0 authorization-server metadata is served at\n    /.well-known/oauth-authorization-server and is byte-identical in substance\n    to the OIDC discovery document (the Auth0 default). Machine-to-machine\n    access would use the client_credentials grant against the same token\n    endpoint, but no resource\
  \ server, audience or API scope is published.\n  flows:\n    authorizationCode:\n      authorizationUrl: https://auth.bekhealth.com/authorize\n      tokenUrl: https://auth.bekhealth.com/oauth/token\n      refreshUrl: https://auth.bekhealth.com/oauth/token\n    clientCredentials:\n      tokenUrl: https://auth.bekhealth.com/oauth/token\ngrant_types_supported:\n- client_credentials\n- authorization_code\n- refresh_token\n- password\n- implicit\n- urn:ietf:params:oauth:grant-type:device_code\n- urn:ietf:params:oauth:grant-type:token-exchange\n- urn:ietf:params:oauth:grant-type:jwt-bearer\n- http://auth0.com/oauth/grant-type/password-realm\n- http://auth0.com/oauth/grant-type/passwordless/otp\n- http://auth0.com/oauth/grant-type/mfa-oob\n- http://auth0.com/oauth/grant-type/mfa-otp\n- http://auth0.com/oauth/grant-type/mfa-recovery-code\ntoken_endpoint_auth_methods_supported:\n- client_secret_basic\n- client_secret_post\n- private_key_jwt\n- none\ncode_challenge_methods_supported:\n- S256\n-\
  \ plain\nid_token_signing_alg_values_supported:\n- HS256\n- RS256\n- PS256\nmfa:\n  supported: true\n  evidence: >-\n    mfa_challenge_endpoint plus the mfa-oob / mfa-otp / mfa-recovery-code Auth0\n    grant types are advertised in the discovery document.\nbackchannel_logout_supported: true\nrequest_parameter_supported: false\ngaps:\n- No API-level authentication documentation is published; docs.bekhealth.com\n  302s to this same issuer for every path.\n- No resource-server audience or API-specific scope is advertised, so the\n  discovery document cannot tell an integrator how to obtain a token for a\n  BEKhealth API.\n- The `implicit` and `password` grants remain enabled on the tenant, both\n  discouraged by OAuth 2.1 / RFC 9700 (BCP for OAuth 2.0 Security).\nx-evidence:\n  fetched: '2026-08-06'\n  probes:\n  - url: https://auth.bekhealth.com/.well-known/openid-configuration\n    http_status: 200\n    content_type: application/json; charset=utf-8\n  - url: https://auth.bekhealth.com/.well-known/oauth-authorization-server\n\
  \    http_status: 200\n    content_type: application/json; charset=utf-8\n  - url: https://docs.bekhealth.com/\n    http_status: 302\n    location: https://auth.bekhealth.com/authorize?client_id=...&response_type=code&scope=openid%20email\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bekhealth/refs/heads/main/authentication/bekhealth-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Healthcare
- Clinical Trials
- Clinical Research
- Electronic Health Records
- Real-World Data
- Artificial Intelligence
- Patient Recruitment
- Life Sciences
- Health Data
---
