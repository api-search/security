---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: medseal.app
  spf: true
hosts:
- cert_expires: Jan 16 11:59:42 2027 GMT
  host: medseal.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MedSeal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MedSeal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MedSeal
provider_slug: medseal-app
slug: medseal-app-domain-security
source_filename: medseal-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: medseal.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 11:59:42 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: medseal.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/medseal-app/security/medseal-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Directory
- Doctors
- Patients
- Reviews
---
