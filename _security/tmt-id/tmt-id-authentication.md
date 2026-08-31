---
api_key_in:
- header
- path
api_specs:
- filename: tmt-id-authenticate-api-openapi.yml
  format: yaml
  label: TMT ID Authenticate API
  slug: tmt-id-authenticate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/openapi/tmt-id-authenticate-api-openapi.yml
- filename: tmt-id-http-api-api-openapi.yml
  format: yaml
  label: TMT ID HTTP API
  slug: tmt-id-http-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/openapi/tmt-id-http-api-api-openapi.yml
- filename: tmt-id-http-api-v1-3-api-openapi.yml
  format: yaml
  label: TMT ID HTTP API v1.3 API
  slug: tmt-id-http-api-v1-3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/openapi/tmt-id-http-api-v1-3-api-openapi.yml
- filename: tmt-id-http-api-v2-0-api-openapi.yml
  format: yaml
  label: TMT ID HTTP API v2.0 API
  slug: tmt-id-http-api-v2-0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/openapi/tmt-id-http-api-v2-0-api-openapi.yml
- filename: tmt-id-network-biometrics-api-openapi.yml
  format: yaml
  label: TMT ID Network Biometrics API
  slug: tmt-id-network-biometrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/openapi/tmt-id-network-biometrics-api-openapi.yml
- filename: tmt-id-service-api-openapi.yml
  format: yaml
  label: TMT ID Service API
  slug: tmt-id-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/openapi/tmt-id-service-api-openapi.yml
- filename: tmt-id-standard-api-call-api-openapi.yml
  format: yaml
  label: TMT ID Standard API Call API
  slug: tmt-id-standard-api-call-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/openapi/tmt-id-standard-api-call-api-openapi.yml
- filename: tmt-id-v2-deprecated-api-openapi.yml
  format: yaml
  label: TMT ID v2 (deprecated) API
  slug: tmt-id-v2-deprecated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/openapi/tmt-id-v2-deprecated-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Tmt Id Authentication
name_suffix: Authentication
oauth_flows: []
overview: TMT ID secures its APIs with apiKey and http across 8 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TMT ID
provider_slug: tmt-id
scheme_count: 8
schemes:
- applies_to: TMT Authenticate API
  description: Client id and client secret presented as HTTP Basic to obtain a PASETO access token.
  name: basic
  scheme: basic
  sources:
  - openapi/tmt-id-authenticate.yml
  type: http
  used_by: POST /oauth/token
- applies_to: TMT Authenticate API
  bearer_format: PASETO
  description: Bearer token returned by POST /oauth/token. PASETO rather than JWT — tokens are not introspectable with standard JWT tooling and there is no published JWKS or OIDC discovery document (both probed, 404/503).
  name: paseto_token
  scheme: bearer
  sources:
  - openapi/tmt-id-authenticate.yml
  type: http
  used_by: POST /get_config, POST /validate, GET /authenticate, GET /authenticate/otp
- applies_to: Network Biometrics API
  description: API Token provided during the onboarding process.
  in: header
  name: token
  parameter: API-Token
  sources:
  - openapi/tmt-id-network-biometrics.yml
  type: apiKey
- applies_to: Network Biometrics API
  description: API Secret provided during the onboarding process.
  in: header
  name: secret
  parameter: API-Secret
  sources:
  - openapi/tmt-id-network-biometrics.yml
  type: apiKey
- applies_to: TMT Verify API, TMT TeleShield API
  description: Declared as a required header PARAMETER on every operation rather than as a components.securitySchemes entry, so generic tooling will not treat it as auth. Obtained from the Viteza portal or from Support during customer onboarding.
  in: header
  name: X-API-Key
  parameter: X-API-Key
  sources:
  - openapi/tmt-id-verify.yml
  - openapi/tmt-id-teleshield.yml
  type: apiKey
- applies_to: TMT Verify API, TMT TeleShield API
  description: Paired secret for X-API-Key. Also declared as a header parameter, not a security scheme.
  in: header
  name: X-API-Secret
  parameter: X-API-Secret
  sources:
  - openapi/tmt-id-verify.yml
  - openapi/tmt-id-teleshield.yml
  type: apiKey
- applies_to: TMT Velocity API, TMT Live API
  description: Velocity (GET /standard/{format}/{key}/{secret}/{number}) and Live (GET /{format}/{key}/{secret}/{number}) carry the API credentials as path segments in the request URL. Credentials in a URL path are logged by proxies, browsers and access logs; consumers should treat these keys as rotatable and never expose these calls to a browser or to an agent that persists URLs. This is a legacy carrier-integration shape, not an artefact of the capture.
  in: path
  name: path-embedded key/secret
  parameter: '{key}/{secret}'
  sources:
  - openapi/tmt-id-velocity.yml
  - openapi/tmt-id-live.yml
  type: apiKey
- applies_to: TMT Score API
  description: openapi/tmt-id-score.yml declares no security scheme and no credential parameter on GET /score/{number}. The product is commercially gated, so the published spec is almost certainly incomplete on auth rather than the endpoint being open.
  name: unauthenticated in spec
  sources:
  - openapi/tmt-id-score.yml
  type: none
slug: tmt-id-authentication
source_filename: tmt-id-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: openapi/tmt-id-authenticate.yml, openapi/tmt-id-network-biometrics.yml, openapi/tmt-id-verify.yml,\n  openapi/tmt-id-teleshield.yml, openapi/tmt-id-velocity.yml, openapi/tmt-id-live.yml\ndocs: https://tmtid.com/developers/\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - path\n  oauth2_flows: []\n  credential_issuance: >-\n    Keys are issued two ways. Self-serve: sign up at the Viteza portal\n    (https://viteza.tmtanalysis.com/register) and receive a key/secret pair with 500 free\n    queries for Live, Velocity and TeleShield Routing. Commercial: for Verify, Score,\n    Authenticate and Network Biometrics the key and secret are delivered by TMT ID Support\n    during a customer onboarding conversation (Network Biometrics additionally requires\n    per-feature use-case pre-approval with the data partners). There is no instant\n    self-service key generation for the full product set.\n  note: >-\n\
  \    Every TMT ID product authenticates with a key + secret PAIR — never a single bearer key —\n    but the transport of that pair differs per product, and two products carry it in the URL\n    path rather than in a header. No product uses OAuth 2.0 or OpenID Connect; the only\n    token-based product, Authenticate, exchanges HTTP Basic credentials for a PASETO bearer\n    token at its own /oauth/token endpoint.\nschemes:\n- name: basic\n  type: http\n  scheme: basic\n  applies_to: TMT Authenticate API\n  used_by: POST /oauth/token\n  description: >-\n    Client id and client secret presented as HTTP Basic to obtain a PASETO access token.\n  sources:\n  - openapi/tmt-id-authenticate.yml\n- name: paseto_token\n  type: http\n  scheme: bearer\n  bearer_format: PASETO\n  applies_to: TMT Authenticate API\n  used_by: POST /get_config, POST /validate, GET /authenticate, GET /authenticate/otp\n  description: >-\n    Bearer token returned by POST /oauth/token. PASETO rather than JWT — tokens are\
  \ not\n    introspectable with standard JWT tooling and there is no published JWKS or OIDC discovery\n    document (both probed, 404/503).\n  sources:\n  - openapi/tmt-id-authenticate.yml\n- name: token\n  type: apiKey\n  in: header\n  parameter: API-Token\n  applies_to: Network Biometrics API\n  description: API Token provided during the onboarding process.\n  sources:\n  - openapi/tmt-id-network-biometrics.yml\n- name: secret\n  type: apiKey\n  in: header\n  parameter: API-Secret\n  applies_to: Network Biometrics API\n  description: API Secret provided during the onboarding process.\n  sources:\n  - openapi/tmt-id-network-biometrics.yml\n- name: X-API-Key\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  applies_to: TMT Verify API, TMT TeleShield API\n  description: >-\n    Declared as a required header PARAMETER on every operation rather than as a\n    components.securitySchemes entry, so generic tooling will not treat it as auth. Obtained\n    from the Viteza portal or from\
  \ Support during customer onboarding.\n  sources:\n  - openapi/tmt-id-verify.yml\n  - openapi/tmt-id-teleshield.yml\n- name: X-API-Secret\n  type: apiKey\n  in: header\n  parameter: X-API-Secret\n  applies_to: TMT Verify API, TMT TeleShield API\n  description: Paired secret for X-API-Key. Also declared as a header parameter, not a security scheme.\n  sources:\n  - openapi/tmt-id-verify.yml\n  - openapi/tmt-id-teleshield.yml\n- name: path-embedded key/secret\n  type: apiKey\n  in: path\n  parameter: '{key}/{secret}'\n  applies_to: TMT Velocity API, TMT Live API\n  description: >-\n    Velocity (GET /standard/{format}/{key}/{secret}/{number}) and Live\n    (GET /{format}/{key}/{secret}/{number}) carry the API credentials as path segments in the\n    request URL. Credentials in a URL path are logged by proxies, browsers and access logs;\n    consumers should treat these keys as rotatable and never expose these calls to a browser\n    or to an agent that persists URLs. This is a legacy carrier-integration\
  \ shape, not an\n    artefact of the capture.\n  sources:\n  - openapi/tmt-id-velocity.yml\n  - openapi/tmt-id-live.yml\n- name: unauthenticated in spec\n  type: none\n  applies_to: TMT Score API\n  description: >-\n    openapi/tmt-id-score.yml declares no security scheme and no credential parameter on\n    GET /score/{number}. The product is commercially gated, so the published spec is\n    almost certainly incomplete on auth rather than the endpoint being open.\n  sources:\n  - openapi/tmt-id-score.yml\ngaps:\n- Only 2 of 7 specs (Authenticate, Network Biometrics) declare components.securitySchemes; the\n  other five express credentials as parameters or omit them entirely.\n- No OpenID Connect discovery, no OAuth 2.0 authorization server metadata, no JWKS, no scopes.\n- No published key-rotation or credential-revocation procedure.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/authentication/tmt-id-authentication.yml
summary_line: apiKey/http · 8 schemes
tags:
- Telecommunications
- United Kingdom
- Identity Verification
- Mobile Identity
- SIM Swap
- Anti-Fraud
- Number Intelligence
- Silent Network Authentication
- GSMA Open Gateway
- Network APIs
- ENUM
- KYC
---
