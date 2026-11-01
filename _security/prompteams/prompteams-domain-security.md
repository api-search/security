---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: prompteams.com
  spf: false
hosts:
- cert_expires: Nov 24 00:01:37 2026 GMT
  host: prompteams.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Prompteams Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prompteams, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Prompteams
provider_slug: prompteams
slug: prompteams-domain-security
source_filename: prompteams-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: prompteams.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 00:01:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: prompteams.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/prompteams/security/prompteams-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artificial Intelligence
- Prompt Management
- Collaboration
- Version Control
- Testing
- Company
---
