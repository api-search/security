---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: doroni.io
  spf: true
hosts:
- cert_expires: Jan  4 04:21:51 2027 GMT
  host: doroni.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Doroni Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Doroni, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Doroni
provider_slug: doroni
slug: doroni-domain-security
source_filename: doroni-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: doroni.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 04:21:51 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: doroni.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/doroni/security/doroni-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AirMobility
- eVTOL
- FlyingCars
- Aerospace
---
