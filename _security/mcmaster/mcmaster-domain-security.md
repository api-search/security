---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mcmaster.ca
  spf: true
hosts:
- cert_expires: Nov  1 23:59:59 2026 GMT
  host: www.mcmaster.ca
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: developer.api.mcmaster.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  5 23:59:59 2026 GMT
  host: library.mcmaster.ca
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mcmaster Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for McMaster University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: McMaster University
provider_slug: mcmaster
slug: mcmaster-domain-security
source_filename: mcmaster-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mcmaster.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 23:59:59 2026 GMT\n  hsts: false\n- host: developer.api.mcmaster.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: library.mcmaster.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: mcmaster.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mcmaster/refs/heads/main/security/mcmaster-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Canada
- Ontario
- Research
- Open Access
- Library
---
