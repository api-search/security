---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hkex.com.hk
  spf: true
hosts:
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: www.hkex.com.hk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: data.hkex.com.hk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hkex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HKEX, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HKEX
provider_slug: hkex
slug: hkex-domain-security
source_filename: hkex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hkex.com.hk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: data.hkex.com.hk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hkex.com.hk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hkex/refs/heads/main/security/hkex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial
- Market Data
- Stocks
- Derivatives
- Exchange
- Real-Time
- Historical Data
- Order Book
- Reference Data
- IPO
---
