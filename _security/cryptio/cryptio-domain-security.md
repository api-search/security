---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cryptio.co
  spf: true
hosts:
- cert_expires: Aug 23 08:12:59 2026 GMT
  host: cryptio.co
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cryptio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cryptio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cryptio
provider_slug: cryptio
slug: cryptio-domain-security
source_filename: cryptio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cryptio.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 08:12:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: cryptio.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cryptio/refs/heads/main/security/cryptio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cryptocurrency
- Crypto Accounting
- Digital Assets
- Blockchain
- Compliance
- Financial Reporting
- ERP
- FinTech
---
