---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kondorfinance.com
  spf: true
hosts:
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: www.kondorfinance.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kondor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kondor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kondor
provider_slug: kondor
slug: kondor-domain-security
source_filename: kondor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kondorfinance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: kondorfinance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kondor/refs/heads/main/security/kondor-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Algorithmic Trading
- Crypto
- Expert Advisors
- Financial
- Fintech
- MetaTrader
- Trading
---
