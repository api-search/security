---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: codesummary.io
  spf: true
hosts:
- cert_expires: Dec  6 19:20:13 2026 GMT
  host: codesummary.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Codesummary Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Code Summary, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Code Summary
provider_slug: codesummary
slug: codesummary-domain-security
source_filename: codesummary-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: codesummary.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 19:20:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: codesummary.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codesummary/refs/heads/main/security/codesummary-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Documentation
- Artificial Intelligence
- Knowledge
- Platform
---
