---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: psiquantum.com
  spf: true
hosts:
- cert_expires: Aug 22 04:11:30 2026 GMT
  host: www.psiquantum.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Psiquantum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PsiQuantum, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PsiQuantum
provider_slug: psiquantum
slug: psiquantum-domain-security
source_filename: psiquantum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.psiquantum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 04:11:30 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: psiquantum.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/psiquantum/refs/heads/main/security/psiquantum-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Quantum Computing
- Photonic Quantum Computing
- Fault Tolerant Quantum Computing
- FTQC
- Single Photon Qubits
- Silicon Photonics
- Quantum Resource Estimation
- Quantum Algorithms
- Quantum Software
- Omega Chipset
- Construct
- Circuit Designer
- Bartiq
- QREF
- Semiconductor
- Hardware
---
