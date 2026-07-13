---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: flashbots.net
  spf: true
hosts:
- cert_expires: Sep  1 03:58:20 2026 GMT
  host: www.flashbots.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 08:59:41 2026 GMT
  host: docs.flashbots.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: relay.flashbots.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flashbots Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flashbots, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Flashbots
provider_slug: flashbots
slug: flashbots-domain-security
source_filename: flashbots-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.flashbots.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 03:58:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.flashbots.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 08:59:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: relay.flashbots.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: flashbots.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flashbots/refs/heads/main/security/flashbots-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- MEV
- Ethereum
- Blockchain
- JSON-RPC
- Relay
- MEV-Boost
- MEV-Share
- Flashbots Protect
- SUAVE
- Block Builders
- Validators
---
