---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wenodo.com
  spf: true
hosts:
- cert_expires: Jan 24 15:56:51 2027 GMT
  host: wenodo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Wenodo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wenodo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Wenodo
provider_slug: wenodo
slug: wenodo-domain-security
source_filename: wenodo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wenodo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 15:56:51 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: wenodo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/wenodo/security/wenodo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Hospitality
- Accounting
- Payroll
- Workforce
- DigitalTransformation
---
