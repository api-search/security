---
api_specs:
- filename: blockchain-com-asyncapi.yml
  format: yaml
  label: Blockchain.com WebSocket APIs
  slug: blockchaincom-websocket-apis
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain/refs/heads/main/asyncapi/blockchain-com-asyncapi.yml
- filename: blockchain-addresses-api-openapi.yml
  format: yaml
  label: Blockchain.com Addresses API
  slug: blockchain-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain/refs/heads/main/openapi/blockchain-addresses-api-openapi.yml
- filename: blockchain-blocks-api-openapi.yml
  format: yaml
  label: Blockchain.com Blocks API
  slug: blockchain-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain/refs/heads/main/openapi/blockchain-blocks-api-openapi.yml
- filename: blockchain-charts-api-openapi.yml
  format: yaml
  label: Blockchain.com Charts API
  slug: blockchain-charts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain/refs/heads/main/openapi/blockchain-charts-api-openapi.yml
- filename: blockchain-market-data-api-openapi.yml
  format: yaml
  label: Blockchain.com Market Data API
  slug: blockchain-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain/refs/heads/main/openapi/blockchain-market-data-api-openapi.yml
- filename: blockchain-network-api-openapi.yml
  format: yaml
  label: Blockchain.com Network API
  slug: blockchain-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain/refs/heads/main/openapi/blockchain-network-api-openapi.yml
- filename: blockchain-payments-api-openapi.yml
  format: yaml
  label: Blockchain.com Payments API
  slug: blockchain-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain/refs/heads/main/openapi/blockchain-payments-api-openapi.yml
- filename: blockchain-pools-api-openapi.yml
  format: yaml
  label: Blockchain.com Pools API
  slug: blockchain-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain/refs/heads/main/openapi/blockchain-pools-api-openapi.yml
- filename: blockchain-stats-api-openapi.yml
  format: yaml
  label: Blockchain.com Stats API
  slug: blockchain-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain/refs/heads/main/openapi/blockchain-stats-api-openapi.yml
- filename: blockchain-trading-api-openapi.yml
  format: yaml
  label: Blockchain.com Trading API
  slug: blockchain-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain/refs/heads/main/openapi/blockchain-trading-api-openapi.yml
- filename: blockchain-transactions-api-openapi.yml
  format: yaml
  label: Blockchain.com Transactions API
  slug: blockchain-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain/refs/heads/main/openapi/blockchain-transactions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: blockchain.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: blockchain.info
  spf: true
hosts:
- cert_expires: Oct 26 23:59:59 2026 GMT
  host: www.blockchain.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 23:59:59 2026 GMT
  host: blockchain.info
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 23:59:59 2026 GMT
  host: api.blockchain.info
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blockchain Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blockchain.com, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Blockchain.com
provider_slug: blockchain
slug: blockchain-domain-security
source_filename: blockchain-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.blockchain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: blockchain.info\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.blockchain.info\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: blockchain.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: blockchain.info\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blockchain/refs/heads/main/security/blockchain-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cryptocurrency
- Bitcoin
- Blockchain Data
- Exchange
- Market Data
- Trading
- Payments
- Public APIs
---
