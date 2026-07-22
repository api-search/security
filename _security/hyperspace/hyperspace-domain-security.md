---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: joinearlybird.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: hyperspace.xyz
  spf: true
hosts:
- cert_expires: Sep 22 15:29:32 2026 GMT
  host: joinearlybird.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 06:35:02 2026 GMT
  host: hyperspace.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hyperspace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hyperspace, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hyperspace
provider_slug: hyperspace
slug: hyperspace-domain-security
source_filename: hyperspace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: joinearlybird.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 15:29:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: hyperspace.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 06:35:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: joinearlybird.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: hyperspace.xyz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyperspace/refs/heads/main/security/hyperspace-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto
- Blockchain
- Web3
- Pre-Mainnet
- Devnet
- Pantera Capital
---
