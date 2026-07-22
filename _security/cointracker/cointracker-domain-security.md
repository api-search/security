---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cointracker.io
  spf: true
hosts:
- cert_expires: Sep 15 09:24:53 2026 GMT
  host: www.cointracker.io
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cointracker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CoinTracker, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CoinTracker
provider_slug: cointracker
slug: cointracker-domain-security
source_filename: cointracker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cointracker.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 09:24:53 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: cointracker.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cointracker/refs/heads/main/security/cointracker-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto
- Cryptocurrency
- Tax
- Portfolio Tracking
- Fintech
- Accounting
- Blockchain
---
