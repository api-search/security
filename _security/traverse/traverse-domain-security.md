---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: traverse.so
  spf: false
hosts:
- cert_expires: Aug 29 07:52:30 2026 GMT
  host: traverse.so
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Traverse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Traverse, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Traverse
provider_slug: traverse
slug: traverse-domain-security
source_filename: traverse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: traverse.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 07:52:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: traverse.so\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/traverse/refs/heads/main/security/traverse-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Training Data
- Data Labeling
- Research Lab
- Frontier Models
- Reinforcement Learning
- Y Combinator
---
