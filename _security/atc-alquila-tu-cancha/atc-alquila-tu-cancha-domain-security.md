---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: atcsports.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: alquilatucancha.com
  spf: true
hosts:
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: atcsports.io
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: alquilatucancha.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Atc Alquila Tu Cancha Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ATC (Alquila tu cancha), probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ATC (Alquila tu cancha)
provider_slug: atc-alquila-tu-cancha
slug: atc-alquila-tu-cancha-domain-security
source_filename: atc-alquila-tu-cancha-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: atcsports.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: false\n- host: alquilatucancha.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: atcsports.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: alquilatucancha.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atc-alquila-tu-cancha/refs/heads/main/security/atc-alquila-tu-cancha-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Sports
- Booking
- Reservations
- Sports Management
- Payments
- Mobile
- SaaS
- LATAM
---
