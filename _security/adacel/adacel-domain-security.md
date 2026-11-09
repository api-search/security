---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: adacel.com
  spf: true
hosts:
- cert_expires: Jan  7 12:01:58 2027 GMT
  host: www.adacel.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Adacel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adacel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Adacel
provider_slug: adacel
slug: adacel-domain-security
source_filename: adacel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.adacel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 12:01:58 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: adacel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/adacel/security/adacel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Air Traffic Management
- Simulation
- Aviation
- Technology
---
