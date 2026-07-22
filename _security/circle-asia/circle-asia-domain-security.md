---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getcircle.ai
  spf: true
hosts:
- cert_expires: Aug 13 07:14:51 2026 GMT
  host: getcircle.ai
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Circle Asia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Circle Asia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Circle Asia
provider_slug: circle-asia
slug: circle-asia-domain-security
source_filename: circle-asia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getcircle.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 07:14:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: getcircle.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/circle-asia/refs/heads/main/security/circle-asia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Payments
- Credit Cards
- Buy Now Pay Later
- Consumer Finance
- Mobile Banking
- Vietnam
- Southeast Asia
---
