---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: champ.aero
  spf: true
hosts:
- cert_expires: Sep 19 10:46:04 2026 GMT
  host: www.champ.aero
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 18 23:59:59 2027 GMT
  host: developer.champ.aero
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Champ Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CHAMP Cargosystems, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CHAMP Cargosystems
provider_slug: champ
slug: champ-domain-security
source_filename: champ-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.champ.aero\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 10:46:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.champ.aero\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 18 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: champ.aero\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/champ/refs/heads/main/security/champ-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Air Cargo
- Airlines
- Booking
- Cargo
- Cargospot
- Freight
- Logistics
- Tracking
---
