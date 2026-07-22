---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: quickpic.co.za
  spf: true
hosts:
- cert_expires: Sep  6 07:25:53 2026 GMT
  host: quickpic.co.za
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quickpic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for quickpic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: quickpic
provider_slug: quickpic
slug: quickpic-domain-security
source_filename: quickpic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quickpic.co.za\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 07:25:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: quickpic.co.za\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quickpic/refs/heads/main/security/quickpic-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Portfolio
- Qiming
- South Africa
- Stub
---
