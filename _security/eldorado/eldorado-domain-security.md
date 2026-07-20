---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: eldorado.io
  spf: true
hosts:
- cert_expires: Sep  8 19:04:39 2026 GMT
  host: eldorado.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 15 23:59:59 2027 GMT
  host: api.eldorado.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eldorado Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eldorado, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Eldorado
provider_slug: eldorado
slug: eldorado-domain-security
source_filename: eldorado-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eldorado.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 19:04:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.eldorado.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 15 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: eldorado.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eldorado/refs/heads/main/security/eldorado-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto Web3
- Stablecoins
- Payments
- Onramp
- Offramp
- Cryptocurrency
- Latin America
- KYC
- Compliance
- Fintech
- Trading
---
