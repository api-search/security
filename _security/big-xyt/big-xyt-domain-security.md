---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: xyt.one
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: big-xyt.com
  spf: true
hosts:
- cert_expires: Oct  9 14:44:49 2026 GMT
  host: xyt.one
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 01:21:24 2026 GMT
  host: docs.big-xyt.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Big Xyt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for big xyt, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: big xyt
provider_slug: big-xyt
slug: big-xyt-domain-security
source_filename: big-xyt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xyt.one\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 14:44:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.big-xyt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 01:21:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: xyt.one\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: big-xyt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/big-xyt/refs/heads/main/security/big-xyt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial
- Market Data
- Tick Data
- Trading
- Analytics
- Equities
- ETFs
- Transaction Cost Analysis
- Liquidity
- Order Book
---
