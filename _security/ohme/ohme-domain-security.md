---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ohme-ev.com
  spf: true
hosts:
- cert_expires: Jan 21 19:27:50 2027 GMT
  host: ohme-ev.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ohme Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ohme, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ohme
provider_slug: ohme
slug: ohme-domain-security
source_filename: ohme-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ohme-ev.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 19:27:50 2027 GMT\n  hsts: null\ndomains:\n- domain: ohme-ev.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ohme/security/ohme-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- EV Charging
- Smart Charging
- Home Chargers
- Mobility Solutions
- Built Environment
---
