---
anonymous_access: false
api_key_in: []
api_specs:
- filename: crawlhive-xyz-dev-api-openapi.yml
  format: yaml
  label: CrawlHive Dev API
  slug: crawlhive-xyz-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crawlhive-xyz/openapi/crawlhive-xyz-dev-api-openapi.yml
- filename: crawlhive-xyz-operator-api-openapi.yml
  format: yaml
  label: CrawlHive Operator API
  slug: crawlhive-xyz-operator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crawlhive-xyz/openapi/crawlhive-xyz-operator-api-openapi.yml
- filename: crawlhive-xyz-token-api-openapi.yml
  format: yaml
  label: CrawlHive Token API
  slug: crawlhive-xyz-token-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crawlhive-xyz/openapi/crawlhive-xyz-token-api-openapi.yml
- filename: crawlhive-xyz-track-api-openapi.yml
  format: yaml
  label: CrawlHive Track API
  slug: crawlhive-xyz-track-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crawlhive-xyz/openapi/crawlhive-xyz-track-api-openapi.yml
- filename: crawlhive-xyz-wallet-api-openapi.yml
  format: yaml
  label: CrawlHive Wallet API
  slug: crawlhive-xyz-wallet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crawlhive-xyz/openapi/crawlhive-xyz-wallet-api-openapi.yml
- filename: crawlhive-xyz-wallets-api-openapi.yml
  format: yaml
  label: CrawlHive Wallets API
  slug: crawlhive-xyz-wallets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crawlhive-xyz/openapi/crawlhive-xyz-wallets-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: CrawlHive Authentication
name_suffix: Authentication
oauth_flows: []
overview: CrawlHive secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CrawlHive
provider_slug: crawlhive-xyz
scheme_count: 3
schemes:
- description: Optional. Personal key (chk_, from crawlhive.xyz/brain), CrawlHive bot key (chb_), OAuth token (cht_) or site session. Limits follow the wallet's tier; burn credits apply after the tier limit.
  header: Authorization
  key_prefixes:
  - kind: personal key
    prefix: chk_
    quote: 'create a key `chk_…` (one per wallet, shown once, stored hashed, rotate or revoke any time). Send it as `Authorization: Bearer chk_…`.'
  - kind: CrawlHive bot key
    prefix: chb_
  - kind: OAuth token
    prefix: cht_
  name: holder
  scheme: bearer
  sources:
  - openapi/crawlhive-xyz-brain-openapi.yml
  - https://raw.githubusercontent.com/h100envy/crawlhive-brain/HEAD/README.md
  type: http
- applies_to: MCP server https://crawlhive.xyz/mcp (cht_ tokens are also accepted by the Brain API)
  description: With OAuth the agent registers itself (RFC 7591), opens crawlhive.xyz/oauth/authorize, and you pick an existing bot or create a new one over the crawlers you choose, then approve with your wallet. PKCE (S256) is required, codes are single-use and live 10 minutes, access tokens last 30 days and refresh tokens rotate on every use.
  documented_only: true
  dynamic_client_registration: RFC 7591
  flows:
  - authorizationCode
  metadata:
  - /.well-known/oauth-protected-resource
  - /.well-known/oauth-authorization-server
  name: oauth (MCP connector)
  pkce: S256
  sources:
  - https://raw.githubusercontent.com/h100envy/crawl-hive/HEAD/README.md
  type: oauth2
- description: when limits and credits run out, the endpoint answers `402 Payment Required` with x402 requirements (USDC on Solana). Any x402 client signs the transfer and repeats the request with the `PAYMENT-SIGNATURE` header.
  name: x402
  sources:
  - https://raw.githubusercontent.com/h100envy/crawlhive-brain/HEAD/README.md
  type: payment
slug: crawlhive-xyz-authentication
source_filename: crawlhive-xyz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://raw.githubusercontent.com/h100envy/crawlhive-brain/HEAD/README.md\ndocs: https://github.com/h100envy/crawlhive-brain#readme\nsummary:\n  types:\n  - http\n  - oauth2\n  anonymous_access: true\n  note: Authentication is optional on the Brain API. Without credentials calls are\n    free under a per-IP limit; a Bearer credential raises limits to the wallet's  tier.\n    Beyond limits and credits, the endpoint answers 402 with x402 payment requirements\n    (no account, no key).\nschemes:\n- name: holder\n  type: http\n  scheme: bearer\n  header: Authorization\n  description: Optional. Personal key (chk_, from crawlhive.xyz/brain), CrawlHive\n    bot key (chb_), OAuth token (cht_) or site session. Limits follow the wallet's\n    tier; burn credits apply after the tier limit.\n  key_prefixes:\n  - prefix: chk_\n    kind: personal key\n    quote: 'create a key `chk_…` (one per wallet, shown once, stored hashed, rotate\n \
  \     or revoke any time). Send it as `Authorization: Bearer chk_…`.'\n  - prefix: chb_\n    kind: CrawlHive bot key\n  - prefix: cht_\n    kind: OAuth token\n  sources:\n  - openapi/crawlhive-xyz-brain-openapi.yml\n  - https://raw.githubusercontent.com/h100envy/crawlhive-brain/HEAD/README.md\n- name: oauth (MCP connector)\n  type: oauth2\n  documented_only: true\n  description: With OAuth the agent registers itself (RFC 7591), opens crawlhive.xyz/oauth/authorize,\n    and you pick an existing bot or create a new one over the crawlers you choose,\n    then approve with your wallet. PKCE (S256) is required, codes are single-use and\n    live 10 minutes, access tokens last 30 days and refresh tokens rotate on every\n    use.\n  flows:\n  - authorizationCode\n  pkce: S256\n  dynamic_client_registration: RFC 7591\n  metadata:\n  - /.well-known/oauth-protected-resource\n  - /.well-known/oauth-authorization-server\n  applies_to: MCP server https://crawlhive.xyz/mcp (cht_ tokens are also accepted\n\
  \    by the Brain API)\n  sources:\n  - https://raw.githubusercontent.com/h100envy/crawl-hive/HEAD/README.md\n- name: x402\n  type: payment\n  description: when limits and credits run out, the endpoint answers `402 Payment\n    Required` with x402 requirements (USDC on Solana). Any x402 client signs the transfer\n    and repeats the request with the `PAYMENT-SIGNATURE` header.\n  sources:\n  - https://raw.githubusercontent.com/h100envy/crawlhive-brain/HEAD/README.md\ndocs_also:\n- https://github.com/h100envy/crawl-hive#readme\n"
source_yaml_url: https://artifacts.apis.io/crawlhive-xyz/authentication/crawlhive-xyz-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- Cryptocurrency
- Memecoin
- Solana
- Security Scanning
- Web3
- MCP
- x402
- Telegram Bot
- Blockchain
---
