---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agile-today.org
  spf: false
hosts:
- cert_expires: Jan 15 10:25:29 2027 GMT
  host: agile-today.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agile Today Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agile Today, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Agile Today
provider_slug: agile-today-org
slug: agile-today-org-domain-security
source_filename: agile-today-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agile-today.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 10:25:29 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: agile-today.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/agile-today-org/security/agile-today-org-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Project Management
- AI Integration
- Methodology
- Open Source
- Public Beta
---
