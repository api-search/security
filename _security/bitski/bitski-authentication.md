---
api_key_in: []
api_specs:
- filename: bitski-activity-api-openapi.yml
  format: yaml
  label: Bitski activity API
  slug: bitski-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitski/refs/heads/main/openapi/bitski-activity-api-openapi.yml
- filename: bitski-commerce-api-openapi.yml
  format: yaml
  label: Bitski Commerce API
  slug: bitski-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitski/refs/heads/main/openapi/bitski-commerce-api-openapi.yml
- filename: bitski-droplinks-api-openapi.yml
  format: yaml
  label: Bitski Droplinks API
  slug: bitski-droplinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitski/refs/heads/main/openapi/bitski-droplinks-api-openapi.yml
- filename: bitski-minting-api-openapi.yml
  format: yaml
  label: Bitski Minting API
  slug: bitski-minting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitski/refs/heads/main/openapi/bitski-minting-api-openapi.yml
- filename: bitski-token-gating-api-openapi.yml
  format: yaml
  label: Bitski Token Gating API
  slug: bitski-token-gating-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitski/refs/heads/main/openapi/bitski-token-gating-api-openapi.yml
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Bitski Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Bitski secures its APIs with oauth2 and http across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Bitski
provider_slug: bitski
scheme_count: 3
schemes:
- description: Client credentials — server-to-server access to NFT Service / WaaS APIs.
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://account.bitski.com/oauth2/token
  name: oauth2
  sources:
  - openapi/bitski-nft-service-openapi-original.json
  type: oauth2
- description: HTTP Basic with base64(CREDENTIAL_ID:CREDENTIAL_SECRET) from the developer portal, documented in the quickstart. Backend-only.
  name: basic
  scheme: basic
  sources:
  - https://docs.bitski.com/wallet-as-a-service/quickstart
  type: http
- description: End-user wallet authentication via OAuth2/OIDC hosted login (SDK-driven), issuer account.bitski.com.
  name: oidc-login
  sources:
  - https://docs.bitski.com/react-sdk/authentication
  type: openIdConnect
slug: bitski-authentication
source_filename: bitski-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/bitski-nft-service-openapi-original.json\ndocs: https://docs.bitski.com/wallet-as-a-service/quickstart\nsummary:\n  types:\n  - oauth2\n  - http\n  oauth2_flows:\n  - clientCredentials\nnotes: >-\n  Bitski's NFT Service / WaaS backend APIs are called from your server with\n  application credentials generated in the developer portal\n  (https://developer.bitski.com) as CREDENTIAL_ID + CREDENTIAL_SECRET. The\n  OpenAPI declares an OAuth2 client-credentials flow (token endpoint\n  https://account.bitski.com/oauth2/token); the docs quickstart also documents\n  HTTP Basic authentication passing base64(CREDENTIAL_ID:CREDENTIAL_SECRET) in\n  the Authorization header. Credentials must be kept server-side. Client-facing\n  wallet login uses OAuth2/OIDC (Sign-In / hosted login) via the JavaScript,\n  React (WaaS), and iOS SDKs.\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://account.bitski.com/oauth2/token\n\
  \    scopes: 1\n  description: Client credentials — server-to-server access to NFT Service / WaaS APIs.\n  sources:\n  - openapi/bitski-nft-service-openapi-original.json\n- name: basic\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic with base64(CREDENTIAL_ID:CREDENTIAL_SECRET) from the developer\n    portal, documented in the quickstart. Backend-only.\n  sources:\n  - https://docs.bitski.com/wallet-as-a-service/quickstart\n- name: oidc-login\n  type: openIdConnect\n  description: >-\n    End-user wallet authentication via OAuth2/OIDC hosted login (SDK-driven),\n    issuer account.bitski.com.\n  sources:\n  - https://docs.bitski.com/react-sdk/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitski/refs/heads/main/authentication/bitski-authentication.yml
summary_line: oauth2/http · 3 schemes
tags:
- Web3
- Crypto Wallet
- Wallet as a Service
- NFT
- Blockchain
- Authentication
- OAuth
- Payments
- Developer Tools
- Company
---
