---
api_specs:
- filename: scan-mainnet.json
  format: json
  label: LayerZero Scan API
  slug: layerzero-scan-api
  spec_type: OpenAPI
  url: https://docs.layerzero.network/openapi/scan-mainnet.json
- filename: scan-testnet.json
  format: json
  label: LayerZero Scan API (Testnet)
  slug: layerzero-scan-api-testnet
  spec_type: OpenAPI
  url: https://docs.layerzero.network/openapi/scan-testnet.json
- filename: vt-api.json
  format: json
  label: LayerZero Value Transfer API
  slug: layerzero-value-transfer-api
  spec_type: OpenAPI
  url: https://docs.layerzero.network/openapi/vt-api.json
- filename: oft-mainnet.json
  format: json
  label: LayerZero OFT Transfer API
  slug: layerzero-oft-transfer-api
  spec_type: OpenAPI
  url: https://docs.layerzero.network/openapi/oft-mainnet.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: layerzero.network
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: layerzero-api.com
  spf: false
hosts:
- cert_expires: Sep 25 16:12:10 2026 GMT
  host: layerzero.network
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 04:41:20 2026 GMT
  host: docs.layerzero.network
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: scan.layerzero-api.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Layerzero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LayerZero, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: LayerZero
provider_slug: layerzero
slug: layerzero-domain-security
source_filename: layerzero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: layerzero.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 16:12:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.layerzero.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 04:41:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: scan.layerzero-api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: layerzero.network\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: layerzero-api.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/layerzero/refs/heads/main/security/layerzero-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Blockchain
- Cross-Chain
- Omnichain
- Interoperability
- Web3
- DeFi
- Messaging
- Token Transfers
---
