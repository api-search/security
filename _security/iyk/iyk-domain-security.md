---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: iyk.app
  spf: true
hosts:
- cert_expires: Oct 16 17:44:43 2026 GMT
  host: iyk.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 17:44:43 2026 GMT
  host: docs.iyk.app
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 17:44:43 2026 GMT
  host: api.iyk.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Iyk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IYK, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: IYK
provider_slug: iyk
slug: iyk-domain-security
source_filename: iyk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iyk.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 17:44:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.iyk.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 17:44:43 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\n- host: api.iyk.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 17:44:43 2026 GMT\n  hsts: null\ndomains:\n- domain: iyk.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iyk/refs/heads/main/security/iyk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- NFC
- Phygital
- Blockchain
- NFT
- POAP
- Chips
- Authentication
- Fan Engagement
- Web3
---
