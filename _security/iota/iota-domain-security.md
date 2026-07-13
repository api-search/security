---
api_specs:
- filename: iota-jsonrpc-openapi.json
  format: json
  label: IOTA Coin Query API
  slug: iota-coin-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-jsonrpc-openapi.json
- filename: iota-jsonrpc-openapi.json
  format: json
  label: IOTA Read API
  slug: iota-read-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-jsonrpc-openapi.json
- filename: iota-jsonrpc-openapi.json
  format: json
  label: IOTA Extended API
  slug: iota-extended-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-jsonrpc-openapi.json
- filename: iota-jsonrpc-openapi.json
  format: json
  label: IOTA Governance Read API
  slug: iota-governance-read-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-jsonrpc-openapi.json
- filename: iota-jsonrpc-openapi.json
  format: json
  label: IOTA Move Utils API
  slug: iota-move-utils-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-jsonrpc-openapi.json
- filename: iota-jsonrpc-openapi.json
  format: json
  label: IOTA Transaction Builder API
  slug: iota-transaction-builder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-jsonrpc-openapi.json
- filename: iota-jsonrpc-openapi.json
  format: json
  label: IOTA Write API
  slug: iota-write-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-jsonrpc-openapi.json
- filename: iota-evm-wasp-openapi.yaml
  format: yaml
  label: IOTA EVM JSON-RPC API
  slug: iota-evm-json-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/openapi/iota-evm-wasp-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: iota.org
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: iota.cafe
  spf: false
hosts:
- cert_expires: Sep 29 01:13:18 2026 GMT
  host: www.iota.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 01:13:18 2026 GMT
  host: docs.iota.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 02:59:25 2026 GMT
  host: api.mainnet.iota.cafe
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Iota Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IOTA, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: IOTA
provider_slug: iota
slug: iota-domain-security
source_filename: iota-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.iota.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 01:13:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.iota.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 01:13:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.mainnet.iota.cafe\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 02:59:25 2026 GMT\n  hsts: null\ndomains:\n- domain: iota.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: iota.cafe\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iota/refs/heads/main/security/iota-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Blockchain
- Distributed Ledger
- Web3
- DeFi
- Cryptocurrency
- Move
- Tangle
---
