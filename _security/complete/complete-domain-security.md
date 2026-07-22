---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: complete.so
  spf: true
hosts:
- cert_expires: Oct  1 05:01:03 2026 GMT
  host: www.complete.so
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Complete Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Complete, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Complete
provider_slug: complete
slug: complete-domain-security
source_filename: complete-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.complete.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 05:01:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: complete.so\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/complete/refs/heads/main/security/complete-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Compensation
- Human Resources
- HR Tech
- Total Rewards
- Compensation Management
- SaaS
---
