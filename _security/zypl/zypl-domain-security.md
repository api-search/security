---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: zypl.ai
  spf: false
hosts:
- cert_expires: Sep  4 15:01:57 2026 GMT
  host: zypl.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zypl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zypl, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Zypl
provider_slug: zypl
slug: zypl-domain-security
source_filename: zypl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zypl.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 15:01:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: zypl.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zypl/refs/heads/main/security/zypl-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Ai
- Fintech
- Machine Learning
- Synthetic Data
- Credit Scoring
- Financial Services
- Risk
---
