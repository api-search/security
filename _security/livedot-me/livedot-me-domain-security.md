---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: livedot.me
  spf: true
hosts:
- cert_expires: Jan 13 14:45:44 2027 GMT
  host: livedot.me
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: livedot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for livedot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: livedot
provider_slug: livedot-me
slug: livedot-me-domain-security
source_filename: livedot-me-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: livedot.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 14:45:44 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: livedot.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/livedot-me/security/livedot-me-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Live Tracking
- Sports
- AI Integration
- Garmin
- Event
---
