---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: horizonquantum.com
  spf: true
hosts:
- cert_expires: Aug 26 21:30:23 2026 GMT
  host: www.horizonquantum.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Horizon Quantum Computing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Horizon Quantum Computing, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Horizon Quantum Computing
provider_slug: horizon-quantum-computing
slug: horizon-quantum-computing-domain-security
source_filename: horizon-quantum-computing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.horizonquantum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 21:30:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: horizonquantum.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/horizon-quantum-computing/refs/heads/main/security/horizon-quantum-computing-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Quantum Computing
- Quantum Software
- Developer Tools
- Integrated Development Environment
- Compiler
- Deep Tech
- Singapore
---
