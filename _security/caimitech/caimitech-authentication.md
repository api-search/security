---
api_key_in: []
auth_types:
- app-credential
- request-signature
- bearer-token
description: ''
kind: authentication
layout: security
method: searched
name: Caimitech Authentication
name_suffix: Authentication
oauth_flows: []
overview: caimitech secures its APIs with app-credential, request-signature, and bearer-token across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: caimitech
provider_slug: caimitech
scheme_count: 3
schemes:
- description: Application key identifying the caller, issued on registration with the Wacai Open Platform. Paired with app_secret for request signing.
  in: body
  name: app_key
  param: app_key
  type: apiKey
- algorithms:
  - MAC
  - RSA
  description: Every request to the API gateway is signed with app_secret. Default algorithm is MAC (HMAC); RSA is supported via a configured public/private key pair. Responses may optionally be signature-verified (验签), and payloads optionally encrypted (DES) via the gateway SDK filter chain.
  encoding: base64
  name: app_secret_signature
  type: signature
- description: 'Token-based access used by older SDKs: an access_token is acquired from app_key/app_secret and refreshed via refresh_token. The higher-version all-in-one SDK bypasses the token and connects directly to the gateway. Callers are advised to cache the token (memcache/redis) and to retry requests themselves after an automatic token refresh.'
  name: access_token
  obtained_via: wacai-token-sdk (TokenService.Get / TokenService.Refresh)
  refreshable: true
  type: bearer-token
slug: caimitech-authentication
source_filename: caimitech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: >-\n  https://github.com/wacai/wacai-open-sdk,\n  https://github.com/wacai/wacai-open-sdk-php,\n  https://github.com/wacai/wacai-open-sdk-csharp,\n  https://github.com/wacai/wacai-gateway-sdk (SDK documentation)\nnotes: >-\n  The Wacai Open Platform (挖财开放平台) does not publish an OpenAPI document, so this\n  profile is captured from the first-party SDK documentation rather than derived\n  from a spec. Access is via an app credential (app_key / app_secret) issued by\n  the open platform, with per-request HMAC signing. Older SDKs additionally use a\n  token service (access_token / refresh_token); the higher-version all-in-one SDK\n  connects directly to the gateway without a token.\nsummary:\n  types:\n    - app-credential\n    - request-signature\n    - bearer-token\n  credential: app_key + app_secret (issued by the Wacai Open Platform)\n  signing: [MAC, RSA]\n  token_service: true\nschemes:\n  - name: app_key\n    type: apiKey\n\
  \    in: body\n    param: app_key\n    description: >-\n      Application key identifying the caller, issued on registration with the\n      Wacai Open Platform. Paired with app_secret for request signing.\n  - name: app_secret_signature\n    type: signature\n    algorithms: [MAC, RSA]\n    encoding: base64\n    description: >-\n      Every request to the API gateway is signed with app_secret. Default\n      algorithm is MAC (HMAC); RSA is supported via a configured public/private\n      key pair. Responses may optionally be signature-verified (验签), and payloads\n      optionally encrypted (DES) via the gateway SDK filter chain.\n  - name: access_token\n    type: bearer-token\n    obtained_via: wacai-token-sdk (TokenService.Get / TokenService.Refresh)\n    refreshable: true\n    description: >-\n      Token-based access used by older SDKs: an access_token is acquired from\n      app_key/app_secret and refreshed via refresh_token. The higher-version\n      all-in-one SDK bypasses the token\
  \ and connects directly to the gateway.\n      Callers are advised to cache the token (memcache/redis) and to retry\n      requests themselves after an automatic token refresh.\ntransport:\n  protocol: HTTPS\n  method: POST\n  content_type: application/json\n  encoding: UTF-8\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caimitech/refs/heads/main/authentication/caimitech-authentication.yml
summary_line: app-credential/request-signature/bearer-token · 3 schemes
tags:
- Company
- FinTech
- Personal Finance
- Wealth Management
- Accounting
- Credit
- Open Platform
- API Gateway
- China
---
