---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: furo.solutions
  spf: true
hosts:
- cert_expires: Jan 10 15:29:07 2027 GMT
  host: furo.solutions
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: furō solutions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for furō solutions, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: furō solutions
provider_slug: furo-solutions
slug: furo-solutions-domain-security
source_filename: furo-solutions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: furo.solutions\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 15:29:07 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: furo.solutions\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/furo-solutions/security/furo-solutions-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Automation
- Data
- Consulting
---
