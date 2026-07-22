---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: vetic.in
  spf: true
hosts:
- cert_expires: Sep  3 07:08:34 2026 GMT
  host: vetic.in
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vetic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vetic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Vetic
provider_slug: vetic
slug: vetic-domain-security
source_filename: vetic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vetic.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 07:08:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: vetic.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vetic/refs/heads/main/security/vetic-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Consumer
- Pet Care
- Veterinary
- Pet Healthcare
- Animal Health
- Mobile App
- India
- Diagnostics
- Pharmacy
---
