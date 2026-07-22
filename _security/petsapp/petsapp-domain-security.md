---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: petsapp.com
  spf: true
hosts:
- cert_expires: Sep 24 23:51:32 2026 GMT
  host: petsapp.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Petsapp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Petsapp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Petsapp
provider_slug: petsapp
slug: petsapp-domain-security
source_filename: petsapp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: petsapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:51:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: petsapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/petsapp/refs/heads/main/security/petsapp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Veterinary
- Practice Management
- Client Communication
- Appointments
- Payments
- Messaging
- SaaS
- Animal Health
---
