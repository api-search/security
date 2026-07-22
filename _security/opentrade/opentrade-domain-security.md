---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: opentrade.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: open-trade.io
  spf: true
hosts:
- cert_expires: Sep 21 20:52:49 2026 GMT
  host: www.opentrade.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 23:59:59 2026 GMT
  host: app.open-trade.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 23:44:23 2026 GMT
  host: docs.opentrade.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opentrade Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Opentrade, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Opentrade
provider_slug: opentrade
slug: opentrade-domain-security
source_filename: opentrade-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.opentrade.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 20:52:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.open-trade.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:59:59 2026 GMT\n  hsts: null\n- host: docs.opentrade.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:44:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: opentrade.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: open-trade.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opentrade/refs/heads/main/security/opentrade-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Stablecoin
- Yield
- Lending
- Treasury Management
- Embedded Finance
- Tokenization
- Real World Assets
- DeFi
- Fintech Infrastructure
- Blockchain
- Fixed Income
---
