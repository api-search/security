---
api_key_in:
- header
api_specs:
- filename: futureverse-rootrewards-quest-api-openapi.yml
  format: yaml
  label: RootRewards Quest API
  slug: rootrewards-quest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/futureverse/refs/heads/main/openapi/futureverse-rootrewards-quest-api-openapi.yml
auth_types:
- openIdConnect
- oauth2
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Futureverse Authentication
name_suffix: Authentication
oauth_flows: []
overview: Futureverse secures its APIs with openIdConnect, oauth2, apiKey, and http across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Futureverse
provider_slug: futureverse
scheme_count: 6
schemes:
- api: FuturePass Identity (OpenID Connect)
  claims:
  - sub
  - iss
  - sid
  - auth_time
  - email
  - profile
  - eoa
  - custodian
  - chainId
  - futurepass
  - connectorId
  - passName
  client_auth_methods:
  - client_secret_basic
  - client_secret_jwt
  - client_secret_post
  - private_key_jwt
  - none
  client_libraries:
  - '@futureverse/auth'
  - '@futureverse/auth-react'
  - '@futureverse/auth-react-native'
  - '@futureverse/next-auth'
  - '@futureverse/oidc-client'
  endpoints:
    authorization: https://login.futureverse.app/auth
    end_session: https://login.futureverse.app/session/end
    introspection: https://login.futureverse.app/token/introspection
    jwks: https://login.futureverse.app/.well-known/jwks.json
    pushed_authorization_request: https://login.futureverse.app/request
    revocation: https://login.futureverse.app/token/revocation
    token: https://login.futureverse.app/token
    userinfo: https://login.futureverse.app/me
  grant_types:
  - authorization_code
  - implicit
  - refresh_token
  - client_credentials
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://login.futureverse.app
  name: futurePassOpenIdConnect
  notes:
  - 'The custom claims are the interesting part: `futurepass` carries the smart-wallet address, `eoa` the externally-owned account behind it, `custodian` the custody provider, `chainId` the network, and `connectorId`/`passName` the social/wallet connector used. That is a deliberate bridge from an OIDC subject to an on-chain identity.'
  - No /.well-known/oauth-authorization-server and no /.well-known/oauth-protected-resource are served (both 404), so the provider is discoverable as OIDC but not as an RFC 8414 / RFC 9728 OAuth server. That matters for MCP clients, which look for those two documents.
  - '`claims_parameter_supported` is false and `request_parameter_supported` is false; PAR is supported instead.'
  openIdConnectUrl: https://login.futureverse.app/.well-known/openid-configuration
  pkce:
  - S256
  response_modes:
  - form_post
  - fragment
  - query
  - web_message
  response_types:
  - code
  - code id_token
  - id_token
  - none
  scopes:
  - openid
  - offline_access
  token_endpoint_auth_signing_algs:
  - HS256
  - RS256
  - PS256
  - ES256
  - EdDSA
  type: openIdConnect
- api: Futureverse Asset Register API
  covers:
  - createSchema
  - registerCollection
  - registerTokenSchema
  - registerSchemaCustomDomain
  - verifySchemaCustomDomain
  - createNamespace
  - createWebhookEndpoint
  - updateWebhookEndpoint
  - deleteWebhookEndpoint
  - createWebhookSubscription
  - deleteWebhookSubscription
  description: Admin ("🔒") functionality on the Asset Register GraphQL API is authenticated with a Sign-In-With-Ethereum (SIWE, EIP-4361) token placed in the Authorization header. Futureverse publishes a browser helper that produces the header value after a wallet signature.
  in: header
  name: assetRegisterSiwe
  note: Introspection and most reads are anonymous — an unauthenticated POST to https://ar-api.futureverse.app/graphql returned the full 186-type schema on 2026-08-16.
  parameter: Authorization
  scheme: bearer
  token_helper: https://ar-docs.futureverse.app/siwe-generator/
  type: http
- api: Futureverse Asset Register API
  description: Asset Register state changes ("🔑") are not authenticated by a token at all. They are submitted as a signed Asset Rights Token Metadata (ARTM) message — a human-readable message following the Ethereum message standard, signed by the asset owner's wallet and submitted via the submitTransaction / assetMutation mutations. Replay protection is a per-address nonce fetched with the getNonceForChainAddress query.
  docs: https://docs.therootnetwork.com/asset-register/guides/asset-register-transaction
  library: '@futureverse/artm'
  message_format: ARTM (Asset Rights Token Metadata)
  name: assetRegisterWalletSignature
  nonce_query: getNonceForChainAddress
  scheme: signature
  type: http
- api: RootRewards Quest API
  description: Quest API key, prefixed `sk_`, bound to the quest owner account. Required on GET /quests/{questId} and POST /quests/{questId}; NOT required on GET /quests or GET /campaigns/{id}. Issued privately on Quest-application approval.
  in: header
  key_prefix: sk_
  name: questApiKey
  parameter: x-api-key
  sources:
  - openapi/futureverse-rootrewards-quest-api-openapi.yml
  - https://docs.therootnetwork.com/rootrewards/api-reference
  type: apiKey
- api: Futureverse Asset Register API
  description: When the Asset Register Subscription Service POSTs an event to a subscriber's webhook endpoint, it sets an API_KEY header so the subscriber can verify the request origin. The key is minted by createWebhookEndpoint and returned as the `apiKey` field.
  direction: inbound-to-subscriber
  docs: https://docs.therootnetwork.com/asset-register/guides/subscriptions
  in: header
  name: webhookDeliveryApiKey
  note: This is a shared-secret header, not a signed payload — there is no HMAC signature scheme (no Stripe-style `t=…,v1=…` header and no timestamp), so a subscriber cannot detect replay.
  parameter: API_KEY
  type: apiKey
- api: The Root Network Node RPC
  description: The public archive nodes at root.rootnet.live and porcini.rootnet.app accept anonymous JSON-RPC POSTs. The documentation warns they are "not for sustained or business use" and recommends running a node or using a third-party RPC service.
  name: nodeRpcAnonymous
  type: none
slug: futureverse-authentication
source_filename: futureverse-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: searched\nsource: >-\n  https://docs.therootnetwork.com/asset-register/authentication (HTTP 200),\n  https://docs.therootnetwork.com/rootrewards/api-reference (HTTP 200), and the live OIDC discovery\n  document at https://login.futureverse.app/.well-known/openid-configuration (HTTP 200, saved to\n  well-known/futureverse-openid-configuration.json). Baseline first derived from\n  openapi/futureverse-rootrewards-quest-api-openapi.yml, then upgraded from the docs and the live\n  discovery document.\ndocs: https://docs.therootnetwork.com/asset-register/authentication\n\nsummary:\n  types:\n    - openIdConnect\n    - oauth2\n    - apiKey\n    - http\n  api_key_in:\n    - header\n  note: >-\n    Three products, three unrelated auth models. Nothing is shared: an OIDC access token from\n    FuturePass is not accepted by the Asset Register, and neither is accepted by RootRewards.\n\nschemes:\n  - name: futurePassOpenIdConnect\n    type: openIdConnect\n\
  \    api: FuturePass Identity (OpenID Connect)\n    openIdConnectUrl: https://login.futureverse.app/.well-known/openid-configuration\n    issuer: https://login.futureverse.app\n    endpoints:\n      authorization: https://login.futureverse.app/auth\n      token: https://login.futureverse.app/token\n      userinfo: https://login.futureverse.app/me\n      introspection: https://login.futureverse.app/token/introspection\n      revocation: https://login.futureverse.app/token/revocation\n      end_session: https://login.futureverse.app/session/end\n      pushed_authorization_request: https://login.futureverse.app/request\n      jwks: https://login.futureverse.app/.well-known/jwks.json\n    grant_types:\n      - authorization_code\n      - implicit\n      - refresh_token\n      - client_credentials\n      - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n    response_types:\n      - code\n      - code id_token\n      - id_token\n      - none\n    response_modes: [form_post, fragment, query, web_message]\n\
  \    pkce: [S256]\n    client_auth_methods:\n      - client_secret_basic\n      - client_secret_jwt\n      - client_secret_post\n      - private_key_jwt\n      - none\n    id_token_signing_alg: [RS256]\n    token_endpoint_auth_signing_algs: [HS256, RS256, PS256, ES256, EdDSA]\n    scopes: [openid, offline_access]\n    claims:\n      - sub\n      - iss\n      - sid\n      - auth_time\n      - email\n      - profile\n      - eoa\n      - custodian\n      - chainId\n      - futurepass\n      - connectorId\n      - passName\n    notes:\n      - >-\n        The custom claims are the interesting part: `futurepass` carries the smart-wallet address,\n        `eoa` the externally-owned account behind it, `custodian` the custody provider, `chainId`\n        the network, and `connectorId`/`passName` the social/wallet connector used. That is a\n        deliberate bridge from an OIDC subject to an on-chain identity.\n      - >-\n        No /.well-known/oauth-authorization-server and no /.well-known/oauth-protected-resource\
  \ are\n        served (both 404), so the provider is discoverable as OIDC but not as an RFC 8414 / RFC 9728\n        OAuth server. That matters for MCP clients, which look for those two documents.\n      - >-\n        `claims_parameter_supported` is false and `request_parameter_supported` is false; PAR is\n        supported instead.\n    client_libraries:\n      - '@futureverse/auth'\n      - '@futureverse/auth-react'\n      - '@futureverse/auth-react-native'\n      - '@futureverse/next-auth'\n      - '@futureverse/oidc-client'\n\n  - name: assetRegisterSiwe\n    type: http\n    scheme: bearer\n    api: Futureverse Asset Register API\n    in: header\n    parameter: Authorization\n    description: >-\n      Admin (\"\U0001F512\") functionality on the Asset Register GraphQL API is authenticated with a\n      Sign-In-With-Ethereum (SIWE, EIP-4361) token placed in the Authorization header. Futureverse\n      publishes a browser helper that produces the header value after a wallet signature.\n\
  \    token_helper: https://ar-docs.futureverse.app/siwe-generator/\n    covers:\n      - createSchema\n      - registerCollection\n      - registerTokenSchema\n      - registerSchemaCustomDomain\n      - verifySchemaCustomDomain\n      - createNamespace\n      - createWebhookEndpoint\n      - updateWebhookEndpoint\n      - deleteWebhookEndpoint\n      - createWebhookSubscription\n      - deleteWebhookSubscription\n    note: >-\n      Introspection and most reads are anonymous — an unauthenticated POST to\n      https://ar-api.futureverse.app/graphql returned the full 186-type schema on 2026-08-16.\n\n  - name: assetRegisterWalletSignature\n    type: http\n    scheme: signature\n    api: Futureverse Asset Register API\n    description: >-\n      Asset Register state changes (\"\U0001F511\") are not authenticated by a token at all. They are\n      submitted as a signed Asset Rights Token Metadata (ARTM) message — a human-readable message\n      following the Ethereum message standard, signed\
  \ by the asset owner's wallet and submitted via\n      the submitTransaction / assetMutation mutations. Replay protection is a per-address nonce\n      fetched with the getNonceForChainAddress query.\n    nonce_query: getNonceForChainAddress\n    message_format: ARTM (Asset Rights Token Metadata)\n    library: '@futureverse/artm'\n    docs: https://docs.therootnetwork.com/asset-register/guides/asset-register-transaction\n\n  - name: questApiKey\n    type: apiKey\n    api: RootRewards Quest API\n    in: header\n    parameter: x-api-key\n    key_prefix: sk_\n    description: >-\n      Quest API key, prefixed `sk_`, bound to the quest owner account. Required on GET\n      /quests/{questId} and POST /quests/{questId}; NOT required on GET /quests or GET\n      /campaigns/{id}. Issued privately on Quest-application approval.\n    sources:\n      - openapi/futureverse-rootrewards-quest-api-openapi.yml\n      - https://docs.therootnetwork.com/rootrewards/api-reference\n\n  - name: webhookDeliveryApiKey\n\
  \    type: apiKey\n    api: Futureverse Asset Register API\n    in: header\n    parameter: API_KEY\n    direction: inbound-to-subscriber\n    description: >-\n      When the Asset Register Subscription Service POSTs an event to a subscriber's webhook\n      endpoint, it sets an API_KEY header so the subscriber can verify the request origin. The key\n      is minted by createWebhookEndpoint and returned as the `apiKey` field.\n    note: >-\n      This is a shared-secret header, not a signed payload — there is no HMAC signature scheme\n      (no Stripe-style `t=…,v1=…` header and no timestamp), so a subscriber cannot detect replay.\n    docs: https://docs.therootnetwork.com/asset-register/guides/subscriptions\n\n  - name: nodeRpcAnonymous\n    type: none\n    api: The Root Network Node RPC\n    description: >-\n      The public archive nodes at root.rootnet.live and porcini.rootnet.app accept anonymous\n      JSON-RPC POSTs. The documentation warns they are \"not for sustained or business\
  \ use\" and\n      recommends running a node or using a third-party RPC service.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/futureverse/refs/heads/main/authentication/futureverse-authentication.yml
summary_line: openIdConnect/oauth2/apiKey/http · 6 schemes
tags:
- Blockchain
- Web3
- Metaverse
- Digital Assets
- NFT
- GraphQL
- Identity
- OpenID Connect
- asset-registry
- Layer 1
- EVM
- Gaming
- agent-native
- MCP
---
