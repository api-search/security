---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cup24.it
  spf: true
hosts:
- cert_expires: Apr  7 23:59:59 2027 GMT
  host: cup24.it
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cup24.it Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cup24.it, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cup24.it
provider_slug: cup24-it
slug: cup24-it-domain-security
source_filename: cup24-it-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cup24.it\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Apr  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cup24.it\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/cup24-it/security/cup24-it-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Healthcare
- Medical Appointments
- Booking
- Marketplace
- Clinics
- Italy
- MCP
---
