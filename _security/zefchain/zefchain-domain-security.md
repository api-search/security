---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: linera.io
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: linera.dev
  spf: false
hosts:
- cert_expires: Sep  7 21:13:03 2026 GMT
  host: linera.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 07:49:49 2026 GMT
  host: linera.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zefchain Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zefchain, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: Zefchain
provider_slug: zefchain
slug: zefchain-domain-security
source_filename: zefchain-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: linera.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 21:13:03 2026 GMT\n  hsts: false\n- host: linera.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 07:49:49 2026 GMT\n  hsts: false\ndomains:\n- domain: linera.io\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n- domain: linera.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zefchain/refs/heads/main/security/zefchain-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Blockchain
- Web3
- Developer Tools
- GraphQL
- Rust
- SDK
- Decentralized Infrastructure
---
