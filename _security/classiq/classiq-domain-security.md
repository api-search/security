---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: classiq.io
  spf: true
hosts:
- cert_expires: Aug 17 11:10:38 2026 GMT
  host: www.classiq.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Classiq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Classiq, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Classiq
provider_slug: classiq
slug: classiq-domain-security
source_filename: classiq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.classiq.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 11:10:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: classiq.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/classiq/refs/heads/main/security/classiq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Quantum Computing
- Quantum Software
- Quantum Algorithm Design
- Quantum Programming Language
- Qmod
- Quantum Synthesis
- Quantum Circuits
- Hardware Agnostic
- Quantum Machine Learning
- Quantum Chemistry
- Quantum Finance
- Quantum Optimization
- Enterprise Quantum
- Python SDK
- AI Assisted Development
---
