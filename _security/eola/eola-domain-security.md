---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: eola.co
  spf: true
hosts:
- cert_expires: Aug 31 04:30:36 2026 GMT
  host: eola.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eola Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for eola, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: eola
provider_slug: eola
slug: eola-domain-security
source_filename: eola-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eola.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 04:30:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: eola.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eola/refs/heads/main/security/eola-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Booking
- Reservations
- Activities
- Leisure
- Experiences
- Tours
- Watersports
- Payments
- SaaS
---
