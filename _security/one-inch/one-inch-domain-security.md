---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: 1inch.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: 1inch.dev
  spf: true
hosts:
- cert_expires: Aug 16 19:25:58 2026 GMT
  host: business.1inch.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 00:36:27 2026 GMT
  host: api.1inch.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: One Inch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 1inch, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: 1inch
provider_slug: one-inch
slug: one-inch-domain-security
source_filename: one-inch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: business.1inch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 19:25:58 2026 GMT\n  hsts: false\n- host: api.1inch.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 00:36:27 2026 GMT\n  hsts: null\ndomains:\n- domain: 1inch.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: 1inch.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/one-inch/refs/heads/main/security/one-inch-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Web3
- DeFi
- DEX
- Aggregator
- Swap
- Multi-chain
- Limit Orders
- Fusion
- Cross-chain
---
