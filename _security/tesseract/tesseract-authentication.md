---
api_key_in: []
api_specs:
- filename: tesseract-public-api-openapi.json
  format: json
  label: Tesseract Public API
  slug: tesseract-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesseract/refs/heads/main/openapi/tesseract-public-api-openapi.json
auth_types:
- none
- signature
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Tesseract Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Tesseract secures its APIs with none, signature, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Tesseract
provider_slug: tesseract
scheme_count: 3
schemes:
- applies_to:
  - openapi/tesseract-public-api-openapi.json
  description: Read endpoints on the Tesseract Public API require no authentication. The vault contract address (and client wallet address) function as the access key; there is no bearer token or API key for GET operations.
  name: PublicRead
  scope: read
  sources:
  - https://docs.tesseract.fi/dedicated-client-vaults/reference/public-api.md
  type: none
- applies_to:
  - openapi/tesseract-public-api-openapi.json#VaultsController_setStrategy
  description: 'The PUT /vaults/{vault}/strategy operation is authorized off-chain by an EIP-712 typed-data signature (SetStrategy: vaultAddress, strategyId, timestamp) signed by the vault owner. No on-chain transaction or gas is required; signatures expire after a short window (send within minutes of signing).'
  domain:
    chainId: 1
    name: Tesseract Public API
    version: '1'
  name: EIP712Signature
  scheme: eip-712
  sources:
  - https://docs.tesseract.fi/dedicated-client-vaults/reference/public-api.md
  type: signature
- applies_to:
  - earn-api
  description: Partner integrations to the Earn API authenticate with OAuth2 client-credentials (M2M). Partners are issued a Client ID and Client Secret which are exchanged for bearer tokens. Credentials are delivered per environment (Development / Test / Production) via Bitwarden Send.
  flow: clientCredentials
  name: EarnApiOAuth2
  sources:
  - https://docs.tesseract.fi/earn-direct-and-earn-api/earn-api/overview.md
  type: oauth2
slug: tesseract-authentication
source_filename: tesseract-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.tesseract.fi/earn-direct-and-earn-api/earn-api/overview.md\ndocs: https://docs.tesseract.fi/dedicated-client-vaults/reference/public-api.md\nsummary:\n  types: [none, signature, oauth2]\n  api_key_in: []\n  oauth2_flows: [clientCredentials]\n  notes: >-\n    Tesseract exposes two distinct API surfaces with different auth models. The\n    public vault reporting API (api.vault.tesseract.fi) requires no credentials\n    for read endpoints — the vault contract address itself acts as the key —\n    while the single write endpoint (strategy assignment) is authorized by an\n    EIP-712 signature validated against the vault owner. The partner-facing Earn\n    API uses OAuth2 client-credentials (machine-to-machine).\nschemes:\n  - name: PublicRead\n    type: none\n    scope: read\n    description: >-\n      Read endpoints on the Tesseract Public API require no authentication. The\n      vault contract address (and client\
  \ wallet address) function as the access\n      key; there is no bearer token or API key for GET operations.\n    applies_to:\n      - openapi/tesseract-public-api-openapi.json\n    sources: [https://docs.tesseract.fi/dedicated-client-vaults/reference/public-api.md]\n  - name: EIP712Signature\n    type: signature\n    scheme: eip-712\n    description: >-\n      The PUT /vaults/{vault}/strategy operation is authorized off-chain by an\n      EIP-712 typed-data signature (SetStrategy: vaultAddress, strategyId,\n      timestamp) signed by the vault owner. No on-chain transaction or gas is\n      required; signatures expire after a short window (send within minutes of\n      signing).\n    domain:\n      name: Tesseract Public API\n      version: '1'\n      chainId: 1\n    applies_to:\n      - openapi/tesseract-public-api-openapi.json#VaultsController_setStrategy\n    sources: [https://docs.tesseract.fi/dedicated-client-vaults/reference/public-api.md]\n  - name: EarnApiOAuth2\n    type: oauth2\n\
  \    flow: clientCredentials\n    description: >-\n      Partner integrations to the Earn API authenticate with OAuth2\n      client-credentials (M2M). Partners are issued a Client ID and Client Secret\n      which are exchanged for bearer tokens. Credentials are delivered per\n      environment (Development / Test / Production) via Bitwarden Send.\n    applies_to: [earn-api]\n    sources: [https://docs.tesseract.fi/earn-direct-and-earn-api/earn-api/overview.md]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tesseract/refs/heads/main/authentication/tesseract-authentication.yml
summary_line: none/signature/oauth2 · 3 schemes
tags:
- Company
- Fintech
- Cryptocurrency
- DeFi
- Lending
- Yield
- Digital Assets
- Ethereum
- MiCA
- Vaults
- Institutional
---
