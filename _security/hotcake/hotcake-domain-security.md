---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hotcake.app
  spf: true
hosts:
- cert_expires: Mar 16 23:59:59 2027 GMT
  host: hotcake.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hotcake Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for hotcake 夯客, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: hotcake 夯客
provider_slug: hotcake
slug: hotcake-domain-security
source_filename: hotcake-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hotcake.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hotcake.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hotcake/refs/heads/main/security/hotcake-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Beauty
- Wellness
- Appointments
- Booking
- Scheduling
- Membership
- POS
- SaaS
- Taiwan
- LINE
- SMB
---
