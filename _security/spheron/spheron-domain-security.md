---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: spheron.network
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: spheron.ai
  spf: true
hosts:
- cert_expires: Aug 28 06:42:42 2026 GMT
  host: www.spheron.network
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 22:48:10 2026 GMT
  host: docs.spheron.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 04:06:28 2026 GMT
  host: app.spheron.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spheron Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spheron, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Spheron
provider_slug: spheron
slug: spheron-domain-security
source_filename: spheron-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.spheron.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 06:42:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.spheron.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 22:48:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.spheron.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 04:06:28 2026 GMT\n  hsts: false\ndomains:\n- domain: spheron.network\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: spheron.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spheron/refs/heads/main/security/spheron-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Compute
- GPU
- GPU Cloud
- Decentralized Compute
- AI Infrastructure
- NVIDIA
- H100
- B200
- Kubernetes
- Bare Metal
- Marketplace
- DePIN
- Web3
- Stablecoin Payments
- MCP
---
