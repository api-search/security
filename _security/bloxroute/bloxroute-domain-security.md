---
api_specs:
- filename: bloxroute-streams-asyncapi.yml
  format: yaml
  label: bloXroute Solana Trader API
  slug: bloxroute-solana-trader-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloxroute/refs/heads/main/asyncapi/bloxroute-streams-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bloxroute.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: blxrbdn.com
  spf: false
hosts:
- cert_expires: Sep  2 02:23:51 2026 GMT
  host: bloxroute.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 16:32:47 2026 GMT
  host: docs.bloxroute.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 23:11:16 2026 GMT
  host: uk.solana.dex.blxrbdn.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bloxroute Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for bloXroute, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: bloXroute
provider_slug: bloxroute
slug: bloxroute-domain-security
source_filename: bloxroute-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bloxroute.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 02:23:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.bloxroute.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 16:32:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: uk.solana.dex.blxrbdn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:11:16 2026 GMT\n  hsts: null\ndomains:\n- domain: bloxroute.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: blxrbdn.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloxroute/refs/heads/main/security/bloxroute-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto
- Blockchain
- Trading
- MEV
- Solana
- Ethereum
- Low Latency
- Streaming
- Infrastructure
---
