---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dognote.app
  spf: true
hosts:
- cert_expires: Dec  7 12:06:14 2026 GMT
  host: dognote.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dognote App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DogNote, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: DogNote
provider_slug: dognote-app
slug: dognote-app-domain-security
source_filename: dognote-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dognote.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 12:06:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dognote.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/dognote-app/security/dognote-app-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Pets
- Mobile App
- Journals
- Health
- DogNote
---
