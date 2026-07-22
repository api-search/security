---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: saber.so
  spf: true
hosts:
- cert_expires: Sep 13 23:29:54 2026 GMT
  host: app.saber.so
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Saber Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Saber, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Saber
provider_slug: saber
slug: saber-domain-security
source_filename: saber-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: app.saber.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:29:54 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: saber.so\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/saber/refs/heads/main/security/saber-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto Web3
- Solana
- Decentralized Finance
- Stablecoins
- Automated Market Maker
- Blockchain
- SDK
---
