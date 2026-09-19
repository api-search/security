---
api_specs:
- filename: supra-accounts-api-openapi.yml
  format: yaml
  label: Supra Accounts API
  slug: supra-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supra/refs/heads/main/openapi/supra-accounts-api-openapi.yml
- filename: supra-block-api-openapi.yml
  format: yaml
  label: Supra Block API
  slug: supra-block-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supra/refs/heads/main/openapi/supra-block-api-openapi.yml
- filename: supra-consensus-api-openapi.yml
  format: yaml
  label: Supra Consensus API
  slug: supra-consensus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supra/refs/heads/main/openapi/supra-consensus-api-openapi.yml
- filename: supra-events-api-openapi.yml
  format: yaml
  label: Supra Events API
  slug: supra-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supra/refs/heads/main/openapi/supra-events-api-openapi.yml
- filename: supra-faucet-api-openapi.yml
  format: yaml
  label: Supra Faucet API
  slug: supra-faucet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supra/refs/heads/main/openapi/supra-faucet-api-openapi.yml
- filename: supra-proofs-api-openapi.yml
  format: yaml
  label: Supra Proofs API
  slug: supra-proofs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supra/refs/heads/main/openapi/supra-proofs-api-openapi.yml
- filename: supra-tables-api-openapi.yml
  format: yaml
  label: Supra Tables API
  slug: supra-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supra/refs/heads/main/openapi/supra-tables-api-openapi.yml
- filename: supra-transactions-api-openapi.yml
  format: yaml
  label: Supra Transactions API
  slug: supra-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supra/refs/heads/main/openapi/supra-transactions-api-openapi.yml
- filename: supra-version-api-openapi.yml
  format: yaml
  label: Supra Version API
  slug: supra-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supra/refs/heads/main/openapi/supra-version-api-openapi.yml
- filename: supra-view-api-openapi.yml
  format: yaml
  label: Supra View API
  slug: supra-view-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supra/refs/heads/main/openapi/supra-view-api-openapi.yml
- filename: supra-websocket-api-openapi.yml
  format: yaml
  label: Supra Web Socket API
  slug: supra-websocket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supra/refs/heads/main/openapi/supra-websocket-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: supra.com
  spf: true
hosts:
- cert_expires: Nov 23 18:12:49 2026 GMT
  host: supra.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 21:12:04 2026 GMT
  host: docs.supra.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 15:18:38 2026 GMT
  host: rpc-mainnet.supra.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Supra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Supra, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Supra
provider_slug: supra
slug: supra-domain-security
source_filename: supra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: supra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 18:12:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.supra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 21:12:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: rpc-mainnet.supra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 15:18:38 2026 GMT\n  hsts: null\ndomains:\n- domain: supra.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/supra/refs/heads/main/security/supra-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Blockchain
- Layer 1
- Oracle
- Web3
- Market Data
- Smart Contracts
- Verifiable Randomness
- Cross-Chain Bridge
- Automation
- Move
- Cryptocurrency
- DeFi
---
