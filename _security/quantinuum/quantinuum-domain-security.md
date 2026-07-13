---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: quantinuum.com
  spf: true
hosts:
- cert_expires: Sep 29 22:13:11 2026 GMT
  host: www.quantinuum.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 21:27:27 2026 GMT
  host: nexus.quantinuum.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: docs.quantinuum.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quantinuum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quantinuum, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Quantinuum
provider_slug: quantinuum
slug: quantinuum-domain-security
source_filename: quantinuum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.quantinuum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 22:13:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: nexus.quantinuum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 21:27:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.quantinuum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: quantinuum.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quantinuum/refs/heads/main/security/quantinuum-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Quantum Computing
- Trapped Ion
- Quantum Hardware
- Quantum Software
- Quantum Compiler
- Quantum Chemistry
- Quantum Natural Language Processing
- Quantum Random Number Generator
- QIR
- OpenQASM
- Cloud Platform
---
