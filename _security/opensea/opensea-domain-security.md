---
api_specs:
- filename: opensea-account-endpoints-api-openapi.yml
  format: yaml
  label: OpenSea Account Endpoints API
  slug: opensea-account-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensea/refs/heads/main/openapi/opensea-account-endpoints-api-openapi.yml
- filename: opensea-analytics-endpoints-api-openapi.yml
  format: yaml
  label: OpenSea Analytics Endpoints API
  slug: opensea-analytics-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensea/refs/heads/main/openapi/opensea-analytics-endpoints-api-openapi.yml
- filename: opensea-auth-endpoints-api-openapi.yml
  format: yaml
  label: OpenSea Auth Endpoints API
  slug: opensea-auth-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensea/refs/heads/main/openapi/opensea-auth-endpoints-api-openapi.yml
- filename: opensea-chain-endpoints-api-openapi.yml
  format: yaml
  label: OpenSea Chain Endpoints API
  slug: opensea-chain-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensea/refs/heads/main/openapi/opensea-chain-endpoints-api-openapi.yml
- filename: opensea-collection-endpoints-api-openapi.yml
  format: yaml
  label: OpenSea Collection Endpoints API
  slug: opensea-collection-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensea/refs/heads/main/openapi/opensea-collection-endpoints-api-openapi.yml
- filename: opensea-contract-endpoints-api-openapi.yml
  format: yaml
  label: OpenSea Contract Endpoints API
  slug: opensea-contract-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensea/refs/heads/main/openapi/opensea-contract-endpoints-api-openapi.yml
- filename: opensea-drops-endpoints-api-openapi.yml
  format: yaml
  label: OpenSea Drops Endpoints API
  slug: opensea-drops-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensea/refs/heads/main/openapi/opensea-drops-endpoints-api-openapi.yml
- filename: opensea-listing-endpoints-api-openapi.yml
  format: yaml
  label: OpenSea Listing Endpoints API
  slug: opensea-listing-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensea/refs/heads/main/openapi/opensea-listing-endpoints-api-openapi.yml
- filename: opensea-nft-endpoints-api-openapi.yml
  format: yaml
  label: OpenSea NFT Endpoints API
  slug: opensea-nft-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensea/refs/heads/main/openapi/opensea-nft-endpoints-api-openapi.yml
- filename: opensea-offer-endpoints-api-openapi.yml
  format: yaml
  label: OpenSea Offer Endpoints API
  slug: opensea-offer-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensea/refs/heads/main/openapi/opensea-offer-endpoints-api-openapi.yml
- filename: opensea-order-endpoints-api-openapi.yml
  format: yaml
  label: OpenSea Order Endpoints API
  slug: opensea-order-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensea/refs/heads/main/openapi/opensea-order-endpoints-api-openapi.yml
- filename: opensea-search-endpoints-api-openapi.yml
  format: yaml
  label: OpenSea Search Endpoints API
  slug: opensea-search-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensea/refs/heads/main/openapi/opensea-search-endpoints-api-openapi.yml
- filename: opensea-swap-endpoints-api-openapi.yml
  format: yaml
  label: OpenSea Swap Endpoints API
  slug: opensea-swap-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensea/refs/heads/main/openapi/opensea-swap-endpoints-api-openapi.yml
- filename: opensea-token-endpoints-api-openapi.yml
  format: yaml
  label: OpenSea Token Endpoints API
  slug: opensea-token-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensea/refs/heads/main/openapi/opensea-token-endpoints-api-openapi.yml
- filename: opensea-tool-endpoints-beta-api-openapi.yml
  format: yaml
  label: OpenSea Tool Endpoints [Beta] API
  slug: opensea-tool-endpoints-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensea/refs/heads/main/openapi/opensea-tool-endpoints-beta-api-openapi.yml
- filename: opensea-transaction-endpoints-api-openapi.yml
  format: yaml
  label: OpenSea Transaction Endpoints API
  slug: opensea-transaction-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensea/refs/heads/main/openapi/opensea-transaction-endpoints-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: opensea.io
  spf: true
hosts:
- cert_expires: Aug 16 13:22:37 2026 GMT
  host: docs.opensea.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 03:42:10 2026 GMT
  host: api.opensea.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 03:42:10 2026 GMT
  host: stream-api.opensea.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opensea Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenSea, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: OpenSea
provider_slug: opensea
slug: opensea-domain-security
source_filename: opensea-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.opensea.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 13:22:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.opensea.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 03:42:10 2026 GMT\n  hsts: null\n- host: stream-api.opensea.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 03:42:10 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: opensea.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opensea/refs/heads/main/security/opensea-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- NFT
- Marketplace
- Web3
- Blockchain
- Trading
- Digital Assets
---
