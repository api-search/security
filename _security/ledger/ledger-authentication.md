---
api_key_in:
- cookie
- header
api_specs:
- filename: ledger-swap-provider-openapi.yml
  format: yaml
  label: Ledger Wallet Exchange Provider APIs
  slug: ledger-wallet-exchange-provider-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ledger/refs/heads/main/openapi/ledger-swap-provider-openapi.yml
- filename: ledger-enterprise-vault-openapi.yml
  format: yaml
  label: Ledger Enterprise API (Vault API)
  slug: ledger-enterprise-api-vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ledger/refs/heads/main/openapi/ledger-enterprise-vault-openapi.yml
- filename: ledger-enterprise-multisig-openapi.yml
  format: yaml
  label: Ledger Enterprise Multisig API
  slug: ledger-enterprise-multisig-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ledger/refs/heads/main/openapi/ledger-enterprise-multisig-openapi.yml
auth_types:
- apiKey
- http-bearer
description: ''
kind: authentication
layout: security
method: searched
name: Ledger Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ledger secures its APIs with apiKey and http-bearer across 7 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ledger
provider_slug: ledger
scheme_count: 7
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/ledger-buy-provider-openapi.yml
  type: apiKey
- in: header
  name: defaultApiKey
  parameter: x-api-key
  sources:
  - openapi/ledger-card-provider-openapi.yml
  - openapi/ledger-sell-provider-openapi.yml
  - openapi/ledger-swap-provider-openapi.yml
  type: apiKey
- in: cookie
  name: cookieAuth
  parameter: sessionid
  sources:
  - openapi/ledger-enterprise-multisig-openapi.yml
  type: apiKey
- description: Token-based authentication with required prefix "Token"
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/ledger-enterprise-multisig-openapi.yml
  type: apiKey
- description: (**required**) Username of a registered API User
  in: header
  name: Ledger_API_User
  parameter: X-Ledger-API-User
  sources:
  - openapi/ledger-enterprise-vault-openapi.yml
  type: apiKey
- description: If you've set up your API Key when initializing your LAM, you'll need to include it as a header along with the api user header. For more details, [see step 5 of the get started documentation](https://help.vault.ledger.com/Content/api/api_getstarted.html).
  in: header
  name: Ledger_API_Key
  parameter: X-Ledger-API-Key
  sources:
  - openapi/ledger-enterprise-vault-openapi.yml
  type: apiKey
- description: If you've set up HashiCorp Vault as an authentication service, you'll need to pass the `X-Ledger-Store-Auth-Token` header along with the API user header. For more details see [how to set up HashiCorp Vault with the LAM](https://help.vault.ledger.com/Content/api/hashicorp_vault.html).
  in: header
  name: Ledger_Store_Auth_Token
  parameter: X-Ledger-Store-Auth-Token
  sources:
  - openapi/ledger-enterprise-vault-openapi.yml
  type: apiKey
slug: ledger-authentication
source_filename: ledger-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: searched\nsource: openapi/ledger-buy-provider-openapi.yml, openapi/ledger-card-provider-openapi.yml, openapi/ledger-enterprise-multisig-openapi.yml,\n  openapi/ledger-enterprise-vault-openapi.yml, openapi/ledger-sell-provider-openapi.yml, openapi/ledger-swap-provider-openapi.yml\n  ; upgraded from the docs auth pages\nsummary:\n  types:\n  - apiKey\n  - http-bearer\n  api_key_in:\n  - cookie\n  - header\n  bearer: true\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/ledger-buy-provider-openapi.yml\n- name: defaultApiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/ledger-card-provider-openapi.yml\n  - openapi/ledger-sell-provider-openapi.yml\n  - openapi/ledger-swap-provider-openapi.yml\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: sessionid\n  sources:\n  - openapi/ledger-enterprise-multisig-openapi.yml\n- name: tokenAuth\n  type:\
  \ apiKey\n  in: header\n  parameter: Authorization\n  description: Token-based authentication with required prefix \"Token\"\n  sources:\n  - openapi/ledger-enterprise-multisig-openapi.yml\n- name: Ledger_API_User\n  type: apiKey\n  in: header\n  parameter: X-Ledger-API-User\n  description: (**required**) Username of a registered API User\n  sources:\n  - openapi/ledger-enterprise-vault-openapi.yml\n- name: Ledger_API_Key\n  type: apiKey\n  in: header\n  parameter: X-Ledger-API-Key\n  description: If you've set up your API Key when initializing your LAM, you'll need to include it as\n    a header along with the api user header. For more details, [see step 5 of the get started documentation](https://help.vault.ledger.com/Content/api/api_getstarted.html).\n  sources:\n  - openapi/ledger-enterprise-vault-openapi.yml\n- name: Ledger_Store_Auth_Token\n  type: apiKey\n  in: header\n  parameter: X-Ledger-Store-Auth-Token\n  description: If you've set up HashiCorp Vault as an authentication service,\
  \ you'll need to pass the\n    `X-Ledger-Store-Auth-Token` header along with the API user header. For more details see [how to set\n    up HashiCorp Vault with the LAM](https://help.vault.ledger.com/Content/api/hashicorp_vault.html).\n  sources:\n  - openapi/ledger-enterprise-vault-openapi.yml\ndocs: https://help.enterprise.ledger.com/api-documentation/getting-started/authentication\ndocs_findings:\n  enterprise_vault:\n    docs: https://help.enterprise.ledger.com/api-documentation/getting-started/authentication\n    two_credential_families: Ledger issues two distinct credential families for two distinct endpoint\n      sets, which the OpenAPI does not distinguish. REPORTING/NOTIFICATION endpoints use X-Ledger-Workspace\n      plus X-Ledger-Reporting-API-Key against https://api.vault.ledger.com. TRANSACTION and governance\n      endpoints use registered API Operators — X-Ledger-API-User plus X-Ledger-API-Key and/or X-Ledger-Store-Auth-Token,\n      and a bearer access token from POST /auth/token.\n\
  \    headers_not_in_spec:\n    - X-Ledger-Workspace\n    - X-Ledger-Reporting-API-Key\n    operator_provisioning: An API Operator is created by an Administrator in the web app (name + public\n      key), confirmed with a Personal Security Device, and must clear quorum acceptance before it is usable.\n      The API key ID and secret are then generated per user. Credentials cannot be self-served.\n    programmatic_approval: 'Approving a governance request as an API user is a local-signature flow, not\n      a shared-secret flow: getChallenge -> verify the decoded payload -> sign with the operator private\n      key (LEDGER_ENTERPRISE_API_PRIVATE_KEY, hex-encoded PEM) -> approve api with the resulting signature.\n      Ledger states the private key never leaves the local machine.'\n    dead_link_note: The authentication page links three times to https://ledger-enterprise-api-portal.redoc.ly/developer-portal/docs/...\n      — that Redocly portal returns 404 on every path as of 2026-08-25,\
  \ so the pages Ledger points readers\n      at for generating reporting API keys and understanding LAM no longer exist.\n  exchange_provider:\n    docs: https://developers.ledger.com/docs/ledger-live/exchange/swap\n    note: 'A per-provider x-api-key shared secret provisioned by Ledger. Additionally, each swap/sell\n      is secured with an application-layer signature independent of transport auth: the partner generates\n      a structured binary payload, signs it with its own private key, and shares the public key with Ledger\n      for verification. The Ledger device then clear-signs the payload.'\n    enumeration_guard: An unknown or unsupported provider is rejected with the same 401 as an invalid\n      key, so a caller cannot discover which providers exist.\n  multisig:\n    docs: https://help.multisig.ledger.com/guides/api-guides/1.-querying-safe-data\n    note: Read endpoints are fully anonymous — \"No private key or API key is needed for read-only queries.\"\n      Writes carry\
  \ Authorization with the literal prefix \"Token\". Authority to move funds is on-chain\n      (Safe owners and threshold), not in the API credential.\n  device:\n    note: The estate-wide authority model is not a bearer credential at all. Every fund-touching action\n      terminates in a physical confirmation on a Ledger device — a Personal Security Device for Ledger\n      Enterprise, a consumer signer for Ledger Wallet. An API credential can PROPOSE; only hardware can\n      APPROVE.\noauth2: false\noauth2_note: No OAuth 2.0 or OpenID Connect anywhere in the estate; scopes/ is therefore not applicable\n  and is intentionally absent.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ledger/refs/heads/main/authentication/ledger-authentication.yml
summary_line: apiKey/http-bearer · 7 schemes
tags:
- Company
- Cryptocurrency
- Digital Assets
- Hardware Wallet
- Self Custody
- Institutional Custody
- Blockchain
- Payments
- Staking
- Security
- Agent Skills
- agent-native
---
