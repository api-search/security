---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: iqm.tech
  spf: true
hosts:
- cert_expires: Sep 30 10:27:12 2026 GMT
  host: iqm.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 11:41:09 2026 GMT
  host: resonance.iqm.tech
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Iqm Quantum Computers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IQM Quantum Computers, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: IQM Quantum Computers
provider_slug: iqm-quantum-computers
slug: iqm-quantum-computers-domain-security
source_filename: iqm-quantum-computers-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iqm.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 10:27:12 2026 GMT\n  hsts: false\n- host: resonance.iqm.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 11:41:09 2026 GMT\n  hsts: null\ndomains:\n- domain: iqm.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iqm-quantum-computers/refs/heads/main/security/iqm-quantum-computers-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Quantum Computing
- Quantum Cloud
- High Performance Computing
- Research
- Scientific Computing
- Developer Tools
- Protobuf
- Hardware
- Finland
- Deep Tech
---
