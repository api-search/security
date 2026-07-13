---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: push.org
  spf: true
hosts:
- cert_expires: Sep 18 06:46:51 2026 GMT
  host: push.org
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 02:24:49 2026 GMT
  host: faucet.push.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Push Protocol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Push Protocol, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Push Protocol
provider_slug: push-protocol
slug: push-protocol-domain-security
source_filename: push-protocol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: push.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 06:46:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: faucet.push.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 02:24:49 2026 GMT\n  hsts: false\ndomains:\n- domain: push.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/push-protocol/refs/heads/main/security/push-protocol-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Web3
- Blockchain
- Layer 1
- Universal Apps
- Cross-Chain
- EVM
- Solana
- Notifications
- Messaging
- Wallet Abstraction
- Fee Abstraction
- DeFi
---
