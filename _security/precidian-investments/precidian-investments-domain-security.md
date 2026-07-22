---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: precidian.com
  spf: true
hosts:
- cert_expires: Oct  8 23:47:17 2026 GMT
  host: www.precidian.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Precidian Investments Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Precidian Investments, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Precidian Investments
provider_slug: precidian-investments
slug: precidian-investments-domain-security
source_filename: precidian-investments-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.precidian.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:47:17 2026 GMT\n  hsts: false\ndomains:\n- domain: precidian.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/precidian-investments/refs/heads/main/security/precidian-investments-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Financial Services
- Asset Management
- Exchange Traded Funds
- Mutual Funds
- Fintech
- Investment Products
---
