---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lurq.run
  spf: true
hosts:
- cert_expires: Jan 23 16:46:15 2027 GMT
  host: lurq.run
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: lurq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for lurq, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: lurq
provider_slug: lurq-run
slug: lurq-run-domain-security
source_filename: lurq-run-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lurq.run\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 16:46:15 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lurq.run\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/lurq-run/security/lurq-run-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- npm
- Package Security
- Verification
- Developer Tools
---
