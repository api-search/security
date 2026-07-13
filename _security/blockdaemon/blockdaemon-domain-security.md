---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: blockdaemon.com
  spf: true
hosts:
- cert_expires: Sep  1 18:44:37 2026 GMT
  host: www.blockdaemon.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 06:40:12 2026 GMT
  host: docs.blockdaemon.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blockdaemon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blockdaemon, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Blockdaemon
provider_slug: blockdaemon
slug: blockdaemon-domain-security
source_filename: blockdaemon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.blockdaemon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 18:44:37 2026 GMT\n  hsts: false\n- host: docs.blockdaemon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 06:40:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: blockdaemon.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blockdaemon/refs/heads/main/security/blockdaemon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Blockchain
- Web3
- Staking
- Validators
- Custody
- MPC
- Wallets
- Nodes
- RPC
- DeFi
- Indexer
- Tokenization
- Institutional
- Crypto
---
