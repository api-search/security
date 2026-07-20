---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kipu-quantum.com
  spf: true
hosts:
- cert_expires: Sep 24 09:50:25 2026 GMT
  host: kipu-quantum.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 09:43:31 2026 GMT
  host: hub.kipu-quantum.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kipu Quantum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kipu Quantum, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kipu Quantum
provider_slug: kipu-quantum
slug: kipu-quantum-domain-security
source_filename: kipu-quantum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kipu-quantum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 09:50:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: hub.kipu-quantum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 09:43:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kipu-quantum.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kipu-quantum/refs/heads/main/security/kipu-quantum-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Deep Tech
- Quantum Computing
- Quantum
- Artificial Intelligence
- Optimization
- Developer Platform
- SDK
- REST API
- Germany
---
