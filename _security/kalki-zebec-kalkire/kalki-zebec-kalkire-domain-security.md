---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: zebec.io
  spf: true
hosts:
- cert_expires: Sep  7 10:49:12 2026 GMT
  host: zebec.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kalki Zebec Kalkire Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zebec Network, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Zebec Network
provider_slug: kalki-zebec-kalkire
slug: kalki-zebec-kalkire-domain-security
source_filename: kalki-zebec-kalkire-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zebec.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 10:49:12 2026 GMT\n  hsts: null\ndomains:\n- domain: zebec.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kalki-zebec-kalkire/refs/heads/main/security/kalki-zebec-kalkire-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Payments
- Payroll
- Blockchain
- Web3
- Crypto
- SDKs
- Solana
- DeFi
---
