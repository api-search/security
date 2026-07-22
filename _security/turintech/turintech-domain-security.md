---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: turintech.ai
  spf: true
hosts:
- cert_expires: Oct 17 15:50:18 2026 GMT
  host: www.turintech.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Turintech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Turintech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Turintech
provider_slug: turintech
slug: turintech-domain-security
source_filename: turintech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.turintech.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 15:50:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: turintech.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/turintech/refs/heads/main/security/turintech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Code Optimization
- Developer Tools
- DevOps
- Large Language Models
- Agentic AI
- CLI
---
