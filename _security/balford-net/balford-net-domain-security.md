---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: balford.net
  spf: true
hosts:
- cert_expires: Jan 25 14:48:38 2027 GMT
  host: balford.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Balford Net Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Balford, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Balford
provider_slug: balford-net
slug: balford-net-domain-security
source_filename: balford-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: balford.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 14:48:38 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: balford.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/balford-net/security/balford-net-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Manufacturing
- Metal Stamping
- CNC Machining
- Solenoid Housings
- China
- Engineering
---
