---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: reekoh.com
  spf: true
hosts:
- cert_expires: Apr 22 23:59:59 2027 GMT
  host: reekoh.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Reekoh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reekoh, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Reekoh
provider_slug: reekoh
slug: reekoh-domain-security
source_filename: reekoh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reekoh.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Apr 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: reekoh.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/reekoh/security/reekoh-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- IoT
- Integration
- Platform
- Cloud
- Autodesk
---
