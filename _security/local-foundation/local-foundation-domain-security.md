---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: local.foundation
  spf: false
hosts:
- cert_expires: Jan 25 13:50:05 2027 GMT
  host: local.foundation
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Local Foundation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Local Foundation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Local Foundation
provider_slug: local-foundation
slug: local-foundation-domain-security
source_filename: local-foundation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: local.foundation\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 13:50:05 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: local.foundation\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/local-foundation/security/local-foundation-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Community
- Research
- Infrastructure
- Ecosystem
- Startups
---
