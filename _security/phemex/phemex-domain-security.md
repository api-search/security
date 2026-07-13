---
api_specs:
- filename: contract.yml
  format: yaml
  label: Phemex Contract Trading API
  slug: phemex-contract-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phemex/refs/heads/main/openapi/contract.yml
- filename: spot.yml
  format: yaml
  label: Phemex Spot Trading API
  slug: phemex-spot-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phemex/refs/heads/main/openapi/spot.yml
- filename: hedged-perpetual.yml
  format: yaml
  label: Phemex Hedged Perpetual API
  slug: phemex-hedged-perpetual-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phemex/refs/heads/main/openapi/hedged-perpetual.yml
- filename: transfer.yml
  format: yaml
  label: Phemex Asset Transfer API
  slug: phemex-asset-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phemex/refs/heads/main/openapi/transfer.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: phemex.com
  spf: true
hosts:
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: api.phemex.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: testnet-api.phemex.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Phemex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Phemex, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Phemex
provider_slug: phemex
slug: phemex-domain-security
source_filename: phemex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.phemex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: null\n- host: testnet-api.phemex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: phemex.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phemex/refs/heads/main/security/phemex-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Cryptocurrency
- Derivatives
- Spot Trading
- Perpetual Contracts
- Futures
- WebSocket
- Market Data
---
