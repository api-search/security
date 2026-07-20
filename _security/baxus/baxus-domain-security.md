---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: baxus.co
  spf: true
hosts:
- cert_expires: Oct 15 00:27:14 2026 GMT
  host: baxus.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 00:27:14 2026 GMT
  host: www.baxus.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 14:45:42 2026 GMT
  host: services.baxus.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Baxus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Baxus, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Baxus
provider_slug: baxus
slug: baxus-domain-security
source_filename: baxus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: baxus.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 00:27:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.baxus.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 00:27:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: services.baxus.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 14:45:42 2026 GMT\n  hsts: null\ndomains:\n- domain: baxus.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/baxus/refs/heads/main/security/baxus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto Web3
- Blockchain
- Solana
- NFT
- Spirits
- Wine
- Whiskey
- Marketplace
- Collectibles
---
