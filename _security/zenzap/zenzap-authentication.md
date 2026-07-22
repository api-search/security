---
api_key_in:
- header
api_specs:
- filename: zenzap-openapi-original.yml
  format: yaml
  label: Zenzap External Integration API
  slug: zenzap-external-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenzap/refs/heads/main/openapi/zenzap-openapi-original.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Zenzap Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: ZenZap secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: ZenZap
provider_slug: zenzap
scheme_count: 3
schemes:
- description: 'Bearer token for the request. Two flavors:


    - **Static API key** — pass your API key (the value returned as `apiKey` when the bot was created). Must be paired with `X-Signature` + `X-Timestamp` (the `hmacSignature` scheme).

    - **OAuth access token** — pass the JWT returned by `POST /oauth/token`. No signature headers are required.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/zenzap-openapi-original.yml
  type: http
- description: HMAC-SHA256 signature for request verification. Required **only** when authenticating with a static API key. Omit when using an OAuth access token.
  in: header
  name: hmacSignature
  parameter: X-Signature
  sources:
  - openapi/zenzap-openapi-original.yml
  type: apiKey
- description: 'OAuth 2.0 `client_credentials` grant for API-key bots. Use the `clientId` and `clientSecret` returned when the bot was created (or rotated) to mint short-lived access tokens. See [Authentication](/api-reference/authentication) for details.


    Access tokens are bearer JWTs and expire after 1 hour. There is no refresh token — re-mint with the client credentials when the token expires.'
  flows:
  - flow: clientCredentials
    scopes: 12
    tokenUrl: https://api.zenzap.co/oauth/token
  name: oauth2ClientCredentials
  sources:
  - openapi/zenzap-openapi-original.yml
  type: oauth2
slug: zenzap-authentication
source_filename: zenzap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/zenzap-openapi-original.yml\ndocs: https://docs.zenzap.co/api-reference/authentication\nnotes: >-\n  Two credential types work against the same /v2/* endpoints: a static API key\n  (Authorization: Bearer + X-Signature HMAC-SHA256 over \"{timestamp}.{body}\" or\n  \"{timestamp}.{uri}\" + X-Timestamp; timestamps >5 min are rejected), or an\n  OAuth 2.0 client_credentials bearer JWT (expires_in default 3600s, no refresh).\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    Bearer token for the request. Two flavors:\n\n    - **Static API key** — pass your API key (the value returned as `apiKey` when the bot was created). Must be paired with `X-Signature` + `X-Timestamp` (the `hmacSignature` scheme).\n    - **OAuth access token** — pass the JWT returned by `POST /oauth/token`.\
  \ No signature headers are required.\n  sources:\n  - openapi/zenzap-openapi-original.yml\n- name: hmacSignature\n  type: apiKey\n  in: header\n  parameter: X-Signature\n  description: HMAC-SHA256 signature for request verification. Required **only** when authenticating\n    with a static API key. Omit when using an OAuth access token.\n  sources:\n  - openapi/zenzap-openapi-original.yml\n- name: oauth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.zenzap.co/oauth/token\n    scopes: 12\n  description: |-\n    OAuth 2.0 `client_credentials` grant for API-key bots. Use the `clientId` and `clientSecret` returned when the bot was created (or rotated) to mint short-lived access tokens. See [Authentication](/api-reference/authentication) for details.\n\n    Access tokens are bearer JWTs and expire after 1 hour. There is no refresh token — re-mint with the client credentials when the token expires.\n  sources:\n  - openapi/zenzap-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenzap/refs/heads/main/authentication/zenzap-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Company
- Ai Ml
- Messaging
- Team Communication
- Collaboration
- Chat
- Bots
- Webhooks
- Productivity
- Tasks
---
