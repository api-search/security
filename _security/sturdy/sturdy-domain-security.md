---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sturdy.finance
  spf: true
hosts:
- cert_expires: Sep  9 01:20:50 2026 GMT
  host: sturdy.finance
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sturdy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sturdy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sturdy
provider_slug: sturdy
slug: sturdy-domain-security
source_filename: sturdy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sturdy.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 01:20:50 2026 GMT\n  hsts: null\ndomains:\n- domain: sturdy.finance\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sturdy/refs/heads/main/security/sturdy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Crypto
- DeFi
- Lending
- Money Market
- Web3
- Smart Contracts
- Blockchain
---
