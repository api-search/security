---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: rallyprotocol.com
  spf: true
hosts:
- cert_expires: Aug 23 03:12:42 2026 GMT
  host: docs.rallyprotocol.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 07:59:59 2026 GMT
  host: www.rallyprotocol.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rally Network Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rally Network, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Rally Network
provider_slug: rally-network
slug: rally-network-domain-security
source_filename: rally-network-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.rallyprotocol.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 03:12:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.rallyprotocol.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 07:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: rallyprotocol.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rally-network/refs/heads/main/security/rally-network-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Web3
- Blockchain
- SDK
- Mobile
- Wallets
- Gasless Transactions
- Crypto
- Developer Tools
---
