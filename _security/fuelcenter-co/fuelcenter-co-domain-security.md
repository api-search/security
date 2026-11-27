---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fuelcenter.co
  spf: true
hosts:
- cert_expires: Jan  2 21:35:33 2027 GMT
  host: fuelcenter.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FuelCenter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FuelCenter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: FuelCenter
provider_slug: fuelcenter-co
slug: fuelcenter-co-domain-security
source_filename: fuelcenter-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fuelcenter.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 21:35:33 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fuelcenter.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/fuelcenter-co/security/fuelcenter-co-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Endurance
- Marathon
- Fueling
- Calculator
- Runner
---
