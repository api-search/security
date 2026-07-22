---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tradeblock.us
  spf: true
hosts:
- cert_expires: Aug 29 23:01:33 2026 GMT
  host: www.tradeblock.us
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tradeblock Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tradeblock, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Tradeblock
provider_slug: tradeblock
slug: tradeblock-domain-security
source_filename: tradeblock-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tradeblock.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 23:01:33 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: tradeblock.us\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tradeblock/refs/heads/main/security/tradeblock-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Sneakers
- Marketplace
- Trading
- Consumer
- E-Commerce
- Mobile App
- Authentication
- Resale
---
