---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mathwallet.org
  spf: true
hosts:
- cert_expires: Mar 15 11:10:58 2027 GMT
  host: mathwallet.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mathwallet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MathWallet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MathWallet
provider_slug: mathwallet
slug: mathwallet-domain-security
source_filename: mathwallet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mathwallet.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 15 11:10:58 2027 GMT\n  hsts: false\ndomains:\n- domain: mathwallet.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mathwallet/refs/heads/main/security/mathwallet-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Crypto Web3
- Cryptocurrency
- Wallet
- Blockchain
- Web3
- DApps
- Multichain
---
