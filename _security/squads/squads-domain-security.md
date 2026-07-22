---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: squads.xyz
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: squads.so
  spf: false
hosts:
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: squads.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 05:58:38 2026 GMT
  host: docs.squads.so
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: grid.squads.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Squads Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Squads, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Squads
provider_slug: squads
slug: squads-domain-security
source_filename: squads-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: squads.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.squads.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 05:58:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: grid.squads.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: squads.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: squads.so\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/squads/refs/heads/main/security/squads-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Infrastructure
- Blockchain
- Solana
- Multisig
- Smart Accounts
- Stablecoins
- Payments
- Wallet
- Web3
---
