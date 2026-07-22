---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pirislabs.io
  spf: false
hosts:
- cert_expires: Sep  9 23:56:14 2026 GMT
  host: pirislabs.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pirislabs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Piris Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Piris Labs
provider_slug: pirislabs
slug: pirislabs-domain-security
source_filename: pirislabs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pirislabs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:56:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: pirislabs.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pirislabs/refs/heads/main/security/pirislabs-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- Inference
- Networking
- Photonics
- Interconnect
- AI Infrastructure
- GPU Compute
- Low Latency
- Y Combinator
---
