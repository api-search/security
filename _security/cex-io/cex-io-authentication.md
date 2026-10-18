---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cex-io-accounts-api-openapi.yml
  format: yaml
  label: CEX.IO Accounts API
  slug: cex-io-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cex-io/refs/heads/main/openapi/cex-io-accounts-api-openapi.yml
- filename: cex-io-fees-api-openapi.yml
  format: yaml
  label: CEX.IO Fees API
  slug: cex-io-fees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cex-io/refs/heads/main/openapi/cex-io-fees-api-openapi.yml
- filename: cex-io-funding-api-openapi.yml
  format: yaml
  label: CEX.IO Funding API
  slug: cex-io-funding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cex-io/refs/heads/main/openapi/cex-io-funding-api-openapi.yml
- filename: cex-io-history-api-openapi.yml
  format: yaml
  label: CEX.IO History API
  slug: cex-io-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cex-io/refs/heads/main/openapi/cex-io-history-api-openapi.yml
- filename: cex-io-market-data-api-openapi.yml
  format: yaml
  label: CEX.IO Market Data API
  slug: cex-io-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cex-io/refs/heads/main/openapi/cex-io-market-data-api-openapi.yml
- filename: cex-io-orders-api-openapi.yml
  format: yaml
  label: CEX.IO Orders API
  slug: cex-io-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cex-io/refs/heads/main/openapi/cex-io-orders-api-openapi.yml
- filename: cex-io-private-api-openapi.yml
  format: yaml
  label: CEX.IO Private API
  slug: cex-io-private-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cex-io/refs/heads/main/openapi/cex-io-private-api-openapi.yml
- filename: cex-io-public-api-openapi.yml
  format: yaml
  label: CEX.IO Public API
  slug: cex-io-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cex-io/refs/heads/main/openapi/cex-io-public-api-openapi.yml
- filename: cex-io-public-market-data-api-openapi.yml
  format: yaml
  label: CEX.IO Public Market Data API
  slug: cex-io-public-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cex-io/refs/heads/main/openapi/cex-io-public-market-data-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Cex Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: CEX.IO declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: CEX.IO
provider_slug: cex-io
scheme_count: 2
schemes:
- description: Per the docs code example, signature = base64(HMAC-SHA256(apiSecret, action + timestamp + JSON body)), sent with the API key and UNIX timestamp headers to https://trade.cex.io/api/spot/rest/{action}.
  headers:
  - X-AGGR-KEY
  - X-AGGR-TIMESTAMP
  - X-AGGR-SIGNATURE
  in: header
  name: XAggrSignedRequest
  sources:
  - https://trade.cex.io/docs/
  type: apiKey
- description: Legacy Exchange API private methods carry key, signature and nonce (docs.cex.io lists APIkey, nonce and signature request objects).
  in: body
  name: LegacyKeySignatureNonce
  sources:
  - https://docs.cex.io/
  type: apiKey
slug: cex-io-authentication
source_filename: cex-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: searched\nsource: https://trade.cex.io/docs/\ndocs: https://trade.cex.io/docs/\nsummary: CEX.IO Spot Trading private REST calls are signed with an API key and secret using HMAC-SHA256 headers; public calls need no authentication. The legacy Exchange API at cex.io/api uses its own API key, signature and nonce scheme documented at docs.cex.io.\nschemes:\n- name: XAggrSignedRequest\n  type: apiKey\n  in: header\n  headers: [X-AGGR-KEY, X-AGGR-TIMESTAMP, X-AGGR-SIGNATURE]\n  description: Per the docs code example, signature = base64(HMAC-SHA256(apiSecret, action + timestamp + JSON body)), sent with the API key and UNIX timestamp headers to https://trade.cex.io/api/spot/rest/{action}.\n  sources: [https://trade.cex.io/docs/]\n- name: LegacyKeySignatureNonce\n  type: apiKey\n  in: body\n  description: Legacy Exchange API private methods carry key, signature and nonce (docs.cex.io lists APIkey, nonce and signature request objects).\n  sources: [https://docs.cex.io/]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cex-io/refs/heads/main/authentication/cex-io-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Cryptocurrency
- Exchange
- Trading
- Market Data
- WebSocket
- Financial Services
---
