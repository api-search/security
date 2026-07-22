---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: web3.foundation
  spf: true
hosts:
- cert_expires: Sep 21 18:33:51 2026 GMT
  host: web3.foundation
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Web3 Foundation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Web3 Foundation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Web3 Foundation
provider_slug: web3-foundation
slug: web3-foundation-domain-security
source_filename: web3-foundation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: web3.foundation\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 18:33:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: web3.foundation\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/web3-foundation/refs/heads/main/security/web3-foundation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Infrastructure
- Web3
- Blockchain
- Polkadot
- Kusama
- Research
- Grants
- Decentralization
- Nonprofit
---
