---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: 1919.cn
  spf: false
hosts:
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: www.1919.cn
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 1919 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 1919, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: '1919'
provider_slug: '1919'
slug: 1919-domain-security
source_filename: 1919-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.1919.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: 1919.cn\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1919/refs/heads/main/security/1919-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Alcoholic Beverages
- Wine and Spirits
- E-Commerce
- Retail
- Supply Chain
- Logistics
- Marketplace
- Consumer
- China
---
