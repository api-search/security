---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: maystreet.com
  spf: true
hosts:
- cert_expires: Nov  2 23:59:59 2026 GMT
  host: maystreet.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- host: mdx.uat.maystreet.com
  https: false
kind: domain-security
layout: security
method: probed
name: Maystreet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MayStreet, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MayStreet
provider_slug: maystreet
slug: maystreet-domain-security
source_filename: maystreet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: maystreet.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: mdx.uat.maystreet.com\n  https: false\ndomains:\n- domain: maystreet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maystreet/refs/heads/main/security/maystreet-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Financial
- Market Data
- Real-Time
- Trading
- Low Latency
- Tick Data
- Order Book
- Equities
- Options
- Feed Handlers
- PCAP
---
