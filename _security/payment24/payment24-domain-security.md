---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: payment24.co
  spf: true
hosts:
- cert_expires: Jan 25 04:53:10 2027 GMT
  host: payment24.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Payment24 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Payment24, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Payment24
provider_slug: payment24
slug: payment24-domain-security
source_filename: payment24-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: payment24.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 04:53:10 2027 GMT\n  hsts: null\ndomains:\n- domain: payment24.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payment24/refs/heads/main/security/payment24-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Payments
- Fuel Payments
- Fleet Management
- Prepaid Cards
- Loyalty
- Card Issuing
- Acquiring
- Point of Sale
- EV Charging
- Telematics
- Fintech
---
