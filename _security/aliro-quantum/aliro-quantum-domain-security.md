---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aliroquantum.com
  spf: true
hosts:
- cert_expires: Sep 20 00:13:23 2026 GMT
  host: www.aliroquantum.com
  hsts: true
  hsts_max_age: 3628800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aliro Quantum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aliro Quantum, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Aliro Quantum
provider_slug: aliro-quantum
slug: aliro-quantum-domain-security
source_filename: aliro-quantum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aliroquantum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 00:13:23 2026 GMT\n  hsts: true\n  hsts_max_age: 3628800\ndomains:\n- domain: aliroquantum.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aliro-quantum/refs/heads/main/security/aliro-quantum-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Quantum
- Quantum Networking
- Quantum Communications
- Entanglement
- Quantum Internet
- Quantum Key Distribution
- Post-Quantum Security
- Quantum Sensors
- Quantum Computing Interconnect
- Quantum Repeaters
- Network Orchestration
- Network Simulation
- Photonics
- Defense
- Telecommunications
---
