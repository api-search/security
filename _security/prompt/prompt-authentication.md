---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Prompt Authentication
name_suffix: Authentication
oauth_flows: []
overview: Prompt declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Prompt
provider_slug: prompt
scheme_count: 1
schemes:
- backchannel_logout:
    session_supported: true
    supported: true
  client_authentication:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  dpop:
    signing_algs:
    - ES256
    supported: true
  endpoints:
    authorization: https://authenticate.promptemr.com/authorize
    device_authorization: https://authenticate.promptemr.com/oauth/device/code
    dynamic_client_registration: https://authenticate.promptemr.com/oidc/register
    global_token_revocation: https://authenticate.promptemr.com/oauth/global-token-revocation/connection/{connectionName}
    jwks: https://authenticate.promptemr.com/.well-known/jwks.json
    mfa_challenge: https://authenticate.promptemr.com/mfa/challenge
    revocation: https://authenticate.promptemr.com/oauth/revoke
    token: https://authenticate.promptemr.com/oauth/token
    userinfo: https://authenticate.promptemr.com/userinfo
  format: Bearer
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  - password
  - implicit
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  - http://auth0.com/oauth/grant-type/password-realm
  - http://auth0.com/oauth/grant-type/passwordless/otp
  - http://auth0.com/oauth/grant-type/mfa-oob
  - http://auth0.com/oauth/grant-type/mfa-otp
  - http://auth0.com/oauth/grant-type/mfa-recovery-code
  header: Authorization
  id: prompt-oidc
  in: header
  mfa:
    evidence: mfa_challenge_endpoint present in discovery document
    supported: true
  openIdConnectUrl: https://authenticate.promptemr.com/.well-known/openid-configuration
  pkce:
    code_challenge_methods:
    - S256
    - plain
    supported: true
  response_types:
  - code
  - token
  - id_token
  - code token
  - code id_token
  - token id_token
  - code token id_token
  subject_types:
  - public
  token_signing:
    id_token_algs:
    - HS256
    - RS256
    - PS256
    token_endpoint_auth_signing_algs:
    - RS256
    - RS384
    - PS256
  type: openIdConnect
slug: prompt-authentication
source_filename: prompt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://authenticate.promptemr.com/.well-known/openid-configuration\nscope_note: >-\n  Prompt publishes no public API reference, so there is no OpenAPI securitySchemes block to derive\n  from. What IS publicly served, from a host Prompt controls, is the OpenID Connect / RFC 8414\n  discovery document for the identity provider that fronts the Prompt application. This artifact\n  records that surface verbatim from the probe. It describes how a user or a registered client\n  authenticates to Prompt's platform — it does NOT document a public product API, and no public\n  documentation identifies which resource servers accept these tokens.\nprovider:\n  issuer: https://authenticate.promptemr.com/\n  host: authenticate.promptemr.com\n  platform: Auth0 tenant on a Prompt-controlled custom domain\n  reached_from: >-\n    https://go.promptemr.com/ (the Prompt application login) redirects with\n    iss=https%3A%2F%2Fauthenticate.promptemr.com%2F\n\
  schemes:\n- id: prompt-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://authenticate.promptemr.com/.well-known/openid-configuration\n  in: header\n  header: Authorization\n  format: Bearer\n  endpoints:\n    authorization: https://authenticate.promptemr.com/authorize\n    token: https://authenticate.promptemr.com/oauth/token\n    userinfo: https://authenticate.promptemr.com/userinfo\n    jwks: https://authenticate.promptemr.com/.well-known/jwks.json\n    revocation: https://authenticate.promptemr.com/oauth/revoke\n    device_authorization: https://authenticate.promptemr.com/oauth/device/code\n    dynamic_client_registration: https://authenticate.promptemr.com/oidc/register\n    mfa_challenge: https://authenticate.promptemr.com/mfa/challenge\n    global_token_revocation: https://authenticate.promptemr.com/oauth/global-token-revocation/connection/{connectionName}\n  grant_types:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - password\n  - implicit\n  - urn:ietf:params:oauth:grant-type:device_code\n\
  \  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  - http://auth0.com/oauth/grant-type/password-realm\n  - http://auth0.com/oauth/grant-type/passwordless/otp\n  - http://auth0.com/oauth/grant-type/mfa-oob\n  - http://auth0.com/oauth/grant-type/mfa-otp\n  - http://auth0.com/oauth/grant-type/mfa-recovery-code\n  response_types:\n  - code\n  - token\n  - id_token\n  - code token\n  - code id_token\n  - token id_token\n  - code token id_token\n  client_authentication:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - none\n  pkce:\n    supported: true\n    code_challenge_methods:\n    - S256\n    - plain\n  mfa:\n    supported: true\n    evidence: mfa_challenge_endpoint present in discovery document\n  dpop:\n    supported: true\n    signing_algs:\n    - ES256\n  token_signing:\n    id_token_algs:\n    - HS256\n    - RS256\n    - PS256\n    token_endpoint_auth_signing_algs:\n    - RS256\n    - RS384\n    - PS256\n\
  \  backchannel_logout:\n    supported: true\n    session_supported: true\n  subject_types:\n  - public\nobservations:\n- >-\n  `client_credentials` is advertised, which means machine-to-machine tokens are issuable against\n  this tenant — the mechanism an integration API would use. No public documentation names the\n  audience/resource server, so this cannot be confirmed as a customer-usable API path.\n- >-\n  The legacy `password` and `implicit` grants remain enabled on the tenant. Both are discouraged by\n  OAuth 2.1 / RFC 9700 (BCP 240); `password` is disallowed outright.\n- >-\n  `plain` is still listed alongside `S256` in code_challenge_methods_supported, a weaker PKCE\n  challenge method than S256-only.\n- >-\n  HS256 is offered as an id_token signing algorithm alongside RS256/PS256.\n- No security.txt, OAuth protected-resource metadata, or api-catalog is served on any Prompt host.\nx-evidence:\n  fetched: '2026-08-26'\n  url: https://authenticate.promptemr.com/.well-known/openid-configuration\n\
  \  http_status: 200\n  content_type: application/json\n  bytes: 2669\n  saved: well-known/prompt-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prompt/refs/heads/main/authentication/prompt-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Healthcare
- Electronic Medical Records
- Practice Management
- Physical Therapy
- Rehabilitation Therapy
- Health IT
- Medical Billing
- Patient Engagement
- Artificial Intelligence
---
