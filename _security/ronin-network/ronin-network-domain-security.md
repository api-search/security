---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: roninchain.com
  spf: true
hosts:
- cert_expires: Aug 11 06:25:32 2026 GMT
  host: roninchain.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 14:02:56 2026 GMT
  host: docs.roninchain.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 20:04:02 2026 GMT
  host: api.roninchain.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ronin Network Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ronin Network, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ronin Network
provider_slug: ronin-network
slug: ronin-network-domain-security
source_filename: ronin-network-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: roninchain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 06:25:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.roninchain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 14:02:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.roninchain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 20:04:02 2026 GMT\n  hsts: null\ndomains:\n- domain: roninchain.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ronin-network/refs/heads/main/security/ronin-network-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sidechain
- Ethereum
- Gaming
- NFT
- Axie Infinity
- JSON-RPC
- Crypto
- Web3
---
