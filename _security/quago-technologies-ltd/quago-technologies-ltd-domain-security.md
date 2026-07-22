---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: quago.io
  spf: true
hosts:
- cert_expires: Sep 23 23:46:22 2026 GMT
  host: quago.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quago Technologies Ltd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quago Technologies LTD, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Quago Technologies LTD
provider_slug: quago-technologies-ltd
slug: quago-technologies-ltd-domain-security
source_filename: quago-technologies-ltd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quago.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:46:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: quago.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quago-technologies-ltd/refs/heads/main/security/quago-technologies-ltd-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Gaming
- Analytics
- Fraud Detection
- Anti-Cheat
- Machine Learning
- Mobile
- User Acquisition
- SDK
---
