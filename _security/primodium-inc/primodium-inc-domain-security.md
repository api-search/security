---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: primodium.com
  spf: false
hosts:
- cert_expires: Aug 19 17:45:48 2026 GMT
  host: developer.primodium.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Primodium Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Primodium Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Primodium Inc.
provider_slug: primodium-inc
slug: primodium-inc-domain-security
source_filename: primodium-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.primodium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 17:45:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: primodium.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/primodium-inc/refs/heads/main/security/primodium-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Blockchain
- Gaming
- Web3
- Solana
- Ethereum
- GraphQL
- Developer Tools
- Indexer
- Onchain
---
