---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dapperlabs.com
  spf: true
hosts:
- cert_expires: Oct 14 06:59:28 2026 GMT
  host: dapperlabs.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dapperlabs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dapperlabs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Dapperlabs
provider_slug: dapperlabs
slug: dapperlabs-domain-security
source_filename: dapperlabs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dapperlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 06:59:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dapperlabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dapperlabs/refs/heads/main/security/dapperlabs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto
- Blockchain
- NFT
- Digital Collectibles
- Wallet
- Flow
- Smart Contracts
- Gaming
---
