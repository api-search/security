---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wax.io
  spf: true
hosts:
- cert_expires: Oct 12 23:26:35 2026 GMT
  host: wax.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WAX, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: WAX
provider_slug: wax
slug: wax-domain-security
source_filename: wax-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wax.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 23:26:35 2026 GMT\n  hsts: false\ndomains:\n- domain: wax.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wax/refs/heads/main/security/wax-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Crypto
- Blockchain
- NFT
- Web3
- Gaming
- Antelope
- Wallet
---
