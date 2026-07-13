---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: io.net
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: io.solutions
  spf: true
hosts:
- cert_expires: Aug 20 14:50:58 2026 GMT
  host: io.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 16:19:28 2026 GMT
  host: api.intelligence.io.solutions
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 14:50:58 2026 GMT
  host: explorer.io.net
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Io Net Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for io.net, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: io.net
provider_slug: io-net
slug: io-net-domain-security
source_filename: io-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: io.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 14:50:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.intelligence.io.solutions\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 16:19:28 2026 GMT\n  hsts: null\n- host: explorer.io.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 14:50:58 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: io.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: io.solutions\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/io-net/refs/heads/main/security/io-net-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- Artificial Intelligence
- GPU
- Decentralized Compute
- DePIN
- Web3
- Solana
- Inference
- LLM
- Distributed Computing
- Ray
- Kubernetes
- Containers
- Confidential Compute
- Agents
- MCP
---
