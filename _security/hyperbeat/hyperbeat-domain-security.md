---
api_specs:
- filename: hyperbeat-staking-openapi.yml
  format: yaml
  label: Hyperbeat Staking API
  slug: hyperbeat-staking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbeat/refs/heads/main/openapi/hyperbeat-staking-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: hyperbeat.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: p2p.org
  spf: true
hosts:
- cert_expires: Sep 23 07:57:48 2026 GMT
  host: www.hyperbeat.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 15:46:21 2026 GMT
  host: api.p2p.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 03:28:10 2026 GMT
  host: api-test.p2p.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hyperbeat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hyperbeat, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Hyperbeat
provider_slug: hyperbeat
slug: hyperbeat-domain-security
source_filename: hyperbeat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hyperbeat.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 07:57:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.p2p.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 15:46:21 2026 GMT\n  hsts: null\n- host: api-test.p2p.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 03:28:10 2026 GMT\n  hsts: null\ndomains:\n- domain: hyperbeat.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: p2p.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyperbeat/refs/heads/main/security/hyperbeat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- DeFi
- Staking
- Liquid Staking
- Hyperliquid
- HyperEVM
- Blockchain
- Web3
- Cryptocurrency
- Yield
---
