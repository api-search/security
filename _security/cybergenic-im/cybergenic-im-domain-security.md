---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cybergenic.im
  spf: false
hosts:
- cert_expires: Jan  6 12:30:56 2027 GMT
  host: cybergenic.im
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cybergenic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cybergenic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Cybergenic
provider_slug: cybergenic-im
slug: cybergenic-im-domain-security
source_filename: cybergenic-im-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cybergenic.im\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 12:30:56 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cybergenic.im\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/cybergenic-im/security/cybergenic-im-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Oncology
- Genomics
- Data Integration
- Research Platform
---
