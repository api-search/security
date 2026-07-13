---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: xanadu.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pennylane.ai
  spf: true
hosts:
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: www.xanadu.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: pennylane.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 22:23:30 2026 GMT
  host: docs.pennylane.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Xanadu Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xanadu, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Xanadu
provider_slug: xanadu-ai
slug: xanadu-ai-domain-security
source_filename: xanadu-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.xanadu.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: pennylane.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.pennylane.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 22:23:30 2026 GMT\n  hsts: false\ndomains:\n- domain: xanadu.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: pennylane.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xanadu-ai/refs/heads/main/security/xanadu-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Quantum Computing
- Photonic Quantum
- Quantum Machine Learning
- Quantum Chemistry
- Differentiable Programming
- PennyLane
- Open Source
- Compilers
- Simulators
- Continuous Variable
- Gaussian Boson Sampling
- Fault Tolerance
---
