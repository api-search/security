---
api_specs:
- filename: covalent-foundational-api-openapi.yml
  format: yaml
  label: GoldRush Foundational API
  slug: goldrush-foundational-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-foundational-api-openapi.yml
- filename: covalent-streaming-api-openapi.yml
  format: yaml
  label: GoldRush Streaming API
  slug: goldrush-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-streaming-api-openapi.yml
- filename: covalent-pipeline-api-openapi.yml
  format: yaml
  label: GoldRush Pipeline API
  slug: goldrush-pipeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-pipeline-api-openapi.yml
- filename: covalent-hyperliquid-info-api-openapi.yml
  format: yaml
  label: GoldRush Hyperliquid Info API
  slug: goldrush-hyperliquid-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-hyperliquid-info-api-openapi.yml
- filename: covalent-x402-api-openapi.yml
  format: yaml
  label: GoldRush x402 API
  slug: goldrush-x402-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-x402-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: covalenthq.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: goldrush.dev
  spf: true
hosts:
- cert_expires: Sep  4 08:32:44 2026 GMT
  host: www.covalenthq.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 02:11:03 2026 GMT
  host: goldrush.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 14:55:08 2026 GMT
  host: api.covalenthq.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Covalent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Covalent, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Covalent
provider_slug: covalent
slug: covalent-domain-security
source_filename: covalent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.covalenthq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 08:32:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: goldrush.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 02:11:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.covalenthq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 14:55:08 2026 GMT\n  hsts: null\ndomains:\n- domain: covalenthq.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: goldrush.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/security/covalent-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Blockchain
- Web3
- Multi-Chain
- Data Infrastructure
- Crypto
- DeFi
- NFT
- Hyperliquid
- GoldRush
- AI Agents
---
