---
api_key_in:
- header
auth_types:
- http-basic
- bearer-token
- oauth2-sso
- request-signing
description: ''
kind: authentication
layout: security
method: searched
name: Appboxo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Appboxo secures its APIs with http-basic, bearer-token, oauth2-sso, and request-signing across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Appboxo
provider_slug: appboxo
scheme_count: 6
schemes:
- default_prefix: Token
  format: <prefix> base64(hostapp_client_id:hostapp_secret_key)
  header: Authorization
  location: header
  name: hostapp_basic
  scheme: basic
  source: https://docs.boxo.io/host-apps/BoxoPayments
  type: http
  used_on:
  - Get access token (Boxo Connect)
  - Create Order Payment endpoint (Boxo Payments)
  - Get Order Payment Status endpoint (Boxo Payments)
- default_prefix: Token
  format: <prefix> <access_token>
  header: Authorization
  location: header
  name: hostapp_access_token
  notes: 'Access token (+ optional refresh token) obtained via the Boxo Connect "Get access token" exchange; can be used in place of Basic auth on payment requests when "Use access token" is enabled in the Dashboard.

    '
  scheme: bearer
  source: https://docs.boxo.io/host-apps/BoxoConnect
  type: http
- description: 'Boxo Connect is a Single Sign-On flow. The host app issues an authorization code to the Boxo native SDK; the Boxo Platform exchanges it at the host-app backend for an access_token/refresh_token, retrieves user data, and returns a miniapp session token. There are no published OAuth scopes.

    '
  grant: authorization_code
  name: boxo_connect_sso
  source: https://docs.boxo.io/host-apps/BoxoConnect
  tokens:
  - auth_code
  - access_token
  - refresh_token
  - session_token
  type: oauth2
- description: 'Session token returned to the miniapp after Boxo.login(); saved/cleared in the host app via the JS SDK (AppBoxoWebAppSaveToken / AppBoxoWebAppClearToken / AppBoxoWebAppLogin / AppBoxoWebAppLogout).

    '
  name: miniapp_session_token
  scheme: bearer
  source: https://docs.boxo.io/MiniApp%20API%20Reference/AuthenticationAPIRef
  type: http
- algorithms:
  - RSA2
  - HMAC
  - ECDSA
  description: 'Server-to-server requests can be signed and verified. Configurable algorithm (RSA2 / HMAC / ECDSA), hash function (MD5/SHA-1/SHA-224/SHA-256/SHA-384/SHA-512), key format (PEM/DER for RSA2/ECDSA), plus timestamp, optional nonce, identity, client_id and merchant_id in a configurable headers map and signature payload template. Default headers: X-Signature, X-Timestamp, X-Client-Id, X-Nonce, X-Identity, X-Merchant-Id.

    '
  hash_functions:
  - MD5
  - SHA-1
  - SHA-224
  - SHA-256
  - SHA-384
  - SHA-512
  name: request_signaturing
  source: https://docs.boxo.io/host-apps/Signaturing
  type: request-signing
- boxo_egress_ips:
  - 54.254.31.251
  - 18.136.51.105
  description: 'Alternative/complement to request signing for the Boxo->miniapp complete-order webhook: the miniapp backend whitelists Boxo Platform egress IPs.

    '
  name: ip_whitelisting
  source: https://docs.boxo.io/host-apps/Whitelisting
  type: network
slug: appboxo-authentication
source_filename: appboxo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://docs.boxo.io/host-apps/BoxoConnect + /host-apps/BoxoPayments + /host-apps/Signaturing\ndocs: https://docs.boxo.io/host-apps/BoxoConnect\nsummary:\n  types: [http-basic, bearer-token, oauth2-sso, request-signing]\n  api_key_in: [header]\n  notes: >\n    Appboxo (Boxo) is a superapp/miniapp platform. There is no single public REST\n    API with OAuth scopes; auth spans three surfaces: (1) the miniapp<->host JS SDK\n    bridge session token, (2) server-to-server integration auth between the Boxo\n    Platform and host-app backends, and (3) cryptographic request signaturing.\nschemes:\n  - name: hostapp_basic\n    type: http\n    scheme: basic\n    location: header\n    header: Authorization\n    format: \"<prefix> base64(hostapp_client_id:hostapp_secret_key)\"\n    default_prefix: Token\n    used_on:\n      - Get access token (Boxo Connect)\n      - Create Order Payment endpoint (Boxo Payments)\n      - Get Order Payment\
  \ Status endpoint (Boxo Payments)\n    source: https://docs.boxo.io/host-apps/BoxoPayments\n  - name: hostapp_access_token\n    type: http\n    scheme: bearer\n    location: header\n    header: Authorization\n    format: \"<prefix> <access_token>\"\n    default_prefix: Token\n    notes: >\n      Access token (+ optional refresh token) obtained via the Boxo Connect\n      \"Get access token\" exchange; can be used in place of Basic auth on payment\n      requests when \"Use access token\" is enabled in the Dashboard.\n    source: https://docs.boxo.io/host-apps/BoxoConnect\n  - name: boxo_connect_sso\n    type: oauth2\n    grant: authorization_code\n    description: >\n      Boxo Connect is a Single Sign-On flow. The host app issues an authorization\n      code to the Boxo native SDK; the Boxo Platform exchanges it at the host-app\n      backend for an access_token/refresh_token, retrieves user data, and returns a\n      miniapp session token. There are no published OAuth scopes.\n    tokens:\
  \ [auth_code, access_token, refresh_token, session_token]\n    source: https://docs.boxo.io/host-apps/BoxoConnect\n  - name: miniapp_session_token\n    type: http\n    scheme: bearer\n    description: >\n      Session token returned to the miniapp after Boxo.login(); saved/cleared in the\n      host app via the JS SDK (AppBoxoWebAppSaveToken / AppBoxoWebAppClearToken /\n      AppBoxoWebAppLogin / AppBoxoWebAppLogout).\n    source: https://docs.boxo.io/MiniApp%20API%20Reference/AuthenticationAPIRef\n  - name: request_signaturing\n    type: request-signing\n    description: >\n      Server-to-server requests can be signed and verified. Configurable algorithm\n      (RSA2 / HMAC / ECDSA), hash function (MD5/SHA-1/SHA-224/SHA-256/SHA-384/SHA-512),\n      key format (PEM/DER for RSA2/ECDSA), plus timestamp, optional nonce, identity,\n      client_id and merchant_id in a configurable headers map and signature payload\n      template. Default headers: X-Signature, X-Timestamp, X-Client-Id, X-Nonce,\n\
  \      X-Identity, X-Merchant-Id.\n    algorithms: [RSA2, HMAC, ECDSA]\n    hash_functions: [MD5, SHA-1, SHA-224, SHA-256, SHA-384, SHA-512]\n    source: https://docs.boxo.io/host-apps/Signaturing\n  - name: ip_whitelisting\n    type: network\n    description: >\n      Alternative/complement to request signing for the Boxo->miniapp complete-order\n      webhook: the miniapp backend whitelists Boxo Platform egress IPs.\n    boxo_egress_ips: [54.254.31.251, 18.136.51.105]\n    source: https://docs.boxo.io/host-apps/Whitelisting\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appboxo/refs/heads/main/authentication/appboxo-authentication.yml
summary_line: http-basic/bearer-token/oauth2-sso/request-signing · 6 schemes
tags:
- Company
- Super App
- Miniapps
- Mobile SDK
- Embedded Finance
- Payments
- Single Sign-On
- App Platform
- eSIM
- Developer Tools
---
