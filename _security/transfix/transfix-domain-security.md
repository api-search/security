---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: transfix.io
  spf: true
hosts:
- cert_expires: Sep 26 01:28:15 2026 GMT
  host: transfix.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Transfix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transfix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Transfix
provider_slug: transfix
slug: transfix-domain-security
source_filename: transfix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: transfix.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 01:28:15 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: transfix.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transfix/refs/heads/main/security/transfix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Freight
- Freight Technology
- Freight Brokerage
- Transportation Management System
- TMS
- Logistics
- Trucking
- Supply Chain
- SaaS
- AI Pricing
- Rate Prediction
- RFP
- 3PL
- Shippers
- Carriers
---
