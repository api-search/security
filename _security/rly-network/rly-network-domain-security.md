---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rly.network
  spf: true
hosts:
- cert_expires: Sep  2 16:43:06 2026 GMT
  host: rly.network
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rly Network Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RLY Network, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: RLY Network
provider_slug: rly-network
slug: rly-network-domain-security
source_filename: rly-network-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rly.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 16:43:06 2026 GMT\n  hsts: false\ndomains:\n- domain: rly.network\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rly-network/refs/heads/main/security/rly-network-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Web3
- Blockchain
- Wallets
- Mobile SDK
- Gasless Transactions
- Cryptocurrency
- Developer Tools
---
