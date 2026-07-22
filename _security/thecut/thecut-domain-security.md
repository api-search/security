---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: thecut.co
  spf: true
hosts:
- cert_expires: Oct 15 07:00:19 2026 GMT
  host: thecut.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thecut Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for theCut, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: theCut
provider_slug: thecut
slug: thecut-domain-security
source_filename: thecut-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thecut.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 07:00:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: thecut.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thecut/refs/heads/main/security/thecut-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Barbershop
- Booking
- Scheduling
- Appointments
- Marketplace
- Consumer
- Mobile
---
