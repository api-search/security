---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: starmicronics.com
  spf: true
hosts:
- cert_expires: Jan 20 03:39:56 2027 GMT
  host: starmicronics.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Star Micronics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Star Micronics CloudPRNT, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Star Micronics CloudPRNT
provider_slug: star-micronics
slug: star-micronics-domain-security
source_filename: star-micronics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: starmicronics.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 20 03:39:56 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: starmicronics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/star-micronics/security/star-micronics-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- POS
- Hardware
- Printing
- Cloud
- Technology
---
