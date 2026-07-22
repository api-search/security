---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: result.dev
  spf: true
hosts:
- cert_expires: Oct 11 12:18:41 2026 GMT
  host: result.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Result Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Result, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Result
provider_slug: result
slug: result-domain-security
source_filename: result-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: result.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 12:18:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: result.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/result/refs/heads/main/security/result-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Business Operations
- SaaS
- Entrepreneurship
- Payments
- Marketing
- No-Code
- Startups
- Artificial Intelligence
---
