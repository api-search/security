---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: binpress.com
  spf: true
hosts:
- cert_expires: Sep 15 19:12:15 2026 GMT
  host: binpress.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Binpress Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Binpress, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Binpress
provider_slug: binpress
slug: binpress-domain-security
source_filename: binpress-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: binpress.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 19:12:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: binpress.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/binpress/refs/heads/main/security/binpress-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Source Code Marketplace
- Developer Tools
- SDKs
- Software Components
- Digital Goods
- Defunct
---
