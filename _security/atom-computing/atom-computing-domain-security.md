---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: atom-computing.com
  spf: true
hosts:
- cert_expires: Sep 26 19:27:51 2026 GMT
  host: atom-computing.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Atom Computing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atom Computing, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Atom Computing
provider_slug: atom-computing
slug: atom-computing-domain-security
source_filename: atom-computing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: atom-computing.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 19:27:51 2026 GMT\n  hsts: false\ndomains:\n- domain: atom-computing.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atom-computing/refs/heads/main/security/atom-computing-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Quantum Computing
- Neutral Atom
- Gate-Based Quantum
- Logical Qubits
- Error Correction
- Fault Tolerance
- OpenQASM
- QIR
- On-Premises
- Hardware
- Research
---
