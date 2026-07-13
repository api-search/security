---
api_specs:
- filename: quantum-engine-api-openapi.yml
  format: yaml
  label: Google Quantum Engine API
  slug: quantum-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-quantum-ai/refs/heads/main/openapi/quantum-engine-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: quantumai.google
  spf: false
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: googleapis.com
  spf: true
hosts:
- cert_expires: Sep 14 08:35:22 2026 GMT
  host: quantumai.google
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:37:17 2026 GMT
  host: quantum.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:35:22 2026 GMT
  host: www.tensorflow.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Google Quantum Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Quantum AI, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Google Quantum AI
provider_slug: google-quantum-ai
slug: google-quantum-ai-domain-security
source_filename: google-quantum-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quantumai.google\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: quantum.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:37:17 2026 GMT\n  hsts: null\n- host: www.tensorflow.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: quantumai.google\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: false\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-quantum-ai/refs/heads/main/security/google-quantum-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Quantum Computing
- Quantum
- Hardware
- NISQ
- Error Correction
- Willow
- Sycamore
- Cirq
- Quantum Engine
- Superconducting Qubits
- Google Cloud
---
