---
api_key_in: []
auth_types: []
description: A-Mark publishes no developer authentication documentation, but the A-Mark Trading Portal serves a live OAuth 2.0 / OpenID Connect discovery document that describes its token model in full. This artifact is read verbatim from that document plus a probe of the token endpoint itself; nothing here is inferred from prose.
kind: authentication
layout: security
method: probed
name: A Mark Precious Metals Authentication
name_suffix: Authentication
oauth_flows: []
overview: A-Mark Precious Metals declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: A-Mark Precious Metals
provider_slug: a-mark-precious-metals
scheme_count: 2
schemes:
- client_authentication:
  - client_secret_basic
  - client_secret_post
  flow: password
  grant_types:
  - password
  - refresh_token
  issuer: https://portal.amark.com/
  jwks_uri: https://portal.amark.com/.well-known/jwks
  name: OAuth2 Password Grant
  refresh_supported: true
  source: https://portal.amark.com/.well-known/openid-configuration
  token_url: https://portal.amark.com/connect/token
  type: oauth2
- flow: refresh_token
  name: OAuth2 Refresh Token
  source: https://portal.amark.com/.well-known/openid-configuration
  token_url: https://portal.amark.com/connect/token
  type: oauth2
slug: a-mark-precious-metals-authentication
source_filename: a-mark-precious-metals-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: https://portal.amark.com/.well-known/openid-configuration\nprovider: A-Mark Precious Metals\nproviderId: a-mark-precious-metals\ndescription: >-\n  A-Mark publishes no developer authentication documentation, but the A-Mark Trading\n  Portal serves a live OAuth 2.0 / OpenID Connect discovery document that describes its\n  token model in full. This artifact is read verbatim from that document plus a probe of\n  the token endpoint itself; nothing here is inferred from prose.\nsummary: >-\n  OAuth 2.0 Resource Owner Password Credentials (ROPC) with refresh tokens, confidential\n  clients authenticating by client secret. There is no authorization_endpoint, so this is\n  a first-party trading-portal login, not a third-party authorization surface — an\n  integrator cannot obtain a token without A-Mark issuing them portal credentials and a\n  client secret.\nschemes:\n  - name: OAuth2 Password Grant\n    type: oauth2\n    flow: password\n\
  \    token_url: https://portal.amark.com/connect/token\n    issuer: https://portal.amark.com/\n    jwks_uri: https://portal.amark.com/.well-known/jwks\n    client_authentication:\n      - client_secret_basic\n      - client_secret_post\n    grant_types:\n      - password\n      - refresh_token\n    refresh_supported: true\n    source: https://portal.amark.com/.well-known/openid-configuration\n  - name: OAuth2 Refresh Token\n    type: oauth2\n    flow: refresh_token\n    token_url: https://portal.amark.com/connect/token\n    source: https://portal.amark.com/.well-known/openid-configuration\nclaims_supported: [aud, exp, iat, iss, jti, sub]\nsubject_types_supported: [public]\ngaps:\n  - id: no-authorization-endpoint\n    detail: >-\n      The discovery document omits authorization_endpoint, userinfo_endpoint,\n      response_types_supported and id_token_signing_alg_values_supported. Despite\n      advertising the openid scope this is not a usable OIDC authorization-code provider;\n      only\
  \ the direct-credential grant works.\n  - id: empty-jwks\n    detail: >-\n      https://portal.amark.com/.well-known/jwks is served and returns {\"keys\":[]}. No\n      public signing key is published, so a relying party cannot independently verify a\n      token issued by this portal.\n  - id: no-public-docs\n    detail: >-\n      No developer portal, API reference, or written authentication guide was found on\n      amark.com or gold.com. Credentials are issued through the dealer onboarding path\n      (newaccounts@amark.com / trading@amark.com), not self-service.\nx-evidence:\n  - url: https://portal.amark.com/.well-known/openid-configuration\n    http_status: 200\n    content_type: application/json;charset=UTF-8\n    bytes: 575\n  - url: https://portal.amark.com/.well-known/jwks\n    http_status: 200\n    bytes: 11\n  - url: https://portal.amark.com/connect/token\n    http_status: 400\n    note: >-\n      GET returns {\"error\":\"invalid_request\",\"error_description\":\"The specified\
  \ HTTP\n      method is not valid.\"} — a live OAuth 2.0 error envelope confirming the endpoint\n      is real and enforcing POST.\n  - url: https://portal.amark.com/login\n    http_status: 200\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/a-mark-precious-metals/refs/heads/main/authentication/a-mark-precious-metals-authentication.yml
summary_line: 2 schemes
tags:
- Precious Metals
- Trading
- Wholesale
- Gold
- Silver
- Bullion
- Finance
---
