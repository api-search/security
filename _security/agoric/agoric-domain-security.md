---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: agoric.com
  spf: true
hosts:
- cert_expires: Oct 13 16:06:17 2026 GMT
  host: agoric.com
  hsts: true
  hsts_max_age: 7776000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agoric Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agoric, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Agoric
provider_slug: agoric
slug: agoric-domain-security
source_filename: agoric-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agoric.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 16:06:17 2026 GMT\n  hsts: true\n  hsts_max_age: 7776000\ndomains:\n- domain: agoric.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agoric/refs/heads/main/security/agoric-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Smart Contracts
- Blockchain
- JavaScript
- Cosmos
- Orchestration
- Web3
- Cross-Chain
---
