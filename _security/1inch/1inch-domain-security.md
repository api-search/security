---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: 1inch.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: 1inch.dev
  spf: true
hosts:
- cert_expires: Aug 14 09:28:31 2026 GMT
  host: 1inch.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 00:36:27 2026 GMT
  host: portal.1inch.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 19:25:58 2026 GMT
  host: business.1inch.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 1Inch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 1inch, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: 1inch
provider_slug: 1inch
slug: 1inch-domain-security
source_filename: 1inch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 1inch.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 09:28:31 2026 GMT\n  hsts: false\n- host: portal.1inch.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 00:36:27 2026 GMT\n  hsts: false\n- host: business.1inch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 19:25:58 2026 GMT\n  hsts: false\ndomains:\n- domain: 1inch.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: 1inch.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1inch/refs/heads/main/security/1inch-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- DeFi
- DEX Aggregator
- Swap
- Limit Orders
- Fusion
- Web3
- RPC
- Market Data
---
