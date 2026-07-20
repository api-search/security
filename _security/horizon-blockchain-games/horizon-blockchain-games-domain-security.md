---
api_specs:
- filename: horizon-blockchain-games-indexer-openapi-original.json
  format: json
  label: Sequence Indexer API
  slug: sequence-indexer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/horizon-blockchain-games/refs/heads/main/openapi/horizon-blockchain-games-indexer-openapi-original.json
- filename: horizon-blockchain-games-metadata-openapi-original.json
  format: json
  label: Sequence Metadata API
  slug: sequence-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/horizon-blockchain-games/refs/heads/main/openapi/horizon-blockchain-games-metadata-openapi-original.json
- filename: horizon-blockchain-games-marketplace-openapi-original.json
  format: json
  label: Sequence Marketplace API
  slug: sequence-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/horizon-blockchain-games/refs/heads/main/openapi/horizon-blockchain-games-marketplace-openapi-original.json
- filename: horizon-blockchain-games-transactions-openapi-original.json
  format: json
  label: Sequence Transactions (Relayer) API
  slug: sequence-transactions-relayer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/horizon-blockchain-games/refs/heads/main/openapi/horizon-blockchain-games-transactions-openapi-original.json
- filename: horizon-blockchain-games-analytics-openapi-original.json
  format: json
  label: Sequence Analytics API
  slug: sequence-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/horizon-blockchain-games/refs/heads/main/openapi/horizon-blockchain-games-analytics-openapi-original.json
- filename: horizon-blockchain-games-builder-openapi-original.json
  format: json
  label: Sequence Builder API
  slug: sequence-builder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/horizon-blockchain-games/refs/heads/main/openapi/horizon-blockchain-games-builder-openapi-original.json
- filename: horizon-blockchain-games-infrastructure-openapi-original.json
  format: json
  label: Sequence API (Infrastructure)
  slug: sequence-api-infrastructure
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/horizon-blockchain-games/refs/heads/main/openapi/horizon-blockchain-games-infrastructure-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: horizongames.net
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: sequence.app
  spf: false
hosts:
- cert_expires: Sep  9 08:30:39 2026 GMT
  host: horizongames.net
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 30 23:17:27 2026 GMT
  host: api.sequence.app
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 30 23:17:27 2026 GMT
  host: amoy-indexer.sequence.app
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Horizon Blockchain Games Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Horizon Blockchain Games, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Horizon Blockchain Games
provider_slug: horizon-blockchain-games
slug: horizon-blockchain-games-domain-security
source_filename: horizon-blockchain-games-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: horizongames.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  9 08:30:39 2026 GMT\n  hsts: false\n- host: api.sequence.app\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 30 23:17:27 2026 GMT\n  hsts: null\n- host: amoy-indexer.sequence.app\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 30 23:17:27 2026 GMT\n  hsts: null\ndomains:\n- domain: horizongames.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: sequence.app\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/horizon-blockchain-games/refs/heads/main/security/horizon-blockchain-games-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Company
- Consumer
- Blockchain
- Web3
- Gaming
- NFT
- Wallet
- Cryptocurrency
- Smart Contracts
- Marketplace
- Developer Tools
- Ethereum
---
