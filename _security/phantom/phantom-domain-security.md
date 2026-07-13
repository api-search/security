---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: phantom.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: phantom.app
  spf: true
hosts:
- cert_expires: Sep 18 18:52:34 2026 GMT
  host: phantom.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 10 00:13:49 2026 GMT
  host: docs.phantom.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 19:31:44 2026 GMT
  host: phantom.app
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Phantom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Phantom, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Phantom
provider_slug: phantom
slug: phantom-domain-security
source_filename: phantom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: phantom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 18:52:34 2026 GMT\n  hsts: false\n- host: docs.phantom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 00:13:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: phantom.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 19:31:44 2026 GMT\n  hsts: false\ndomains:\n- domain: phantom.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: phantom.app\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phantom/refs/heads/main/security/phantom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Base
- Bitcoin
- Blockchain
- Crypto
- Cryptocurrency
- Deeplinks
- Embedded Wallet
- Ethereum
- EVM
- Monad
- MCP
- Mobile
- Polygon
- Self-Custody
- Solana
- Sui
- Wallet
- Web3
---
