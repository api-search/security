---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pico.net
  spf: true
hosts:
- cert_expires: Oct 11 13:10:13 2026 GMT
  host: www.pico.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 25 13:23:33 2026 GMT
  host: portal.pico.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pico Trading Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pico, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pico
provider_slug: pico-trading
slug: pico-trading-domain-security
source_filename: pico-trading-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pico.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 13:10:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: portal.pico.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 13:23:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: pico.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pico-trading/refs/heads/main/security/pico-trading-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial
- Market Data
- Trading
- Real-Time
- Low Latency
- Feed Handlers
- Order Execution
- Network Analytics
- Exchange Connectivity
---
