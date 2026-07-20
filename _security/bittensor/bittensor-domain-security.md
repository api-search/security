---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bittensor.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: opentensor.ai
  spf: true
hosts:
- cert_expires: Sep 29 18:00:16 2026 GMT
  host: bittensor.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 17:17:21 2026 GMT
  host: www.bittensor.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 18:22:42 2026 GMT
  host: entrypoint-finney.opentensor.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bittensor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bittensor, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bittensor
provider_slug: bittensor
slug: bittensor-domain-security
source_filename: bittensor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bittensor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 18:00:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.bittensor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 17:17:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: entrypoint-finney.opentensor.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 18:22:42 2026 GMT\n  hsts: null\ndomains:\n- domain: bittensor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: opentensor.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bittensor/refs/heads/main/security/bittensor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Blockchain
- Decentralized AI
- Machine Learning
- Cryptocurrency
- Web3
- SDK
- CLI
- DePIN
---
