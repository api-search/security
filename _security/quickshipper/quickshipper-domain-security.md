---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: quickshipper.app
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: qshpr.com
  spf: false
hosts:
- cert_expires: Aug 25 10:57:54 2026 GMT
  host: quickshipper.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 10:57:54 2026 GMT
  host: qshpr.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quickshipper Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quickshipper, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Quickshipper
provider_slug: quickshipper
slug: quickshipper-domain-security
source_filename: quickshipper-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quickshipper.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 10:57:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: qshpr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 10:57:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: quickshipper.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n- domain: qshpr.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quickshipper/refs/heads/main/security/quickshipper-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Logistics
- Last-Mile Delivery
- Fleet Management
- Shipping
- Courier
- Route Optimization
- SaaS
---
