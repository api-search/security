---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: 1stdibs.com
  spf: true
hosts:
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: 1stdibs.com
  hsts: true
  hsts_max_age: 63113852
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 1Stdibs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 1stdibs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: 1stdibs
provider_slug: 1stdibs
slug: 1stdibs-domain-security
source_filename: 1stdibs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 1stdibs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63113852\ndomains:\n- domain: 1stdibs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1stdibs/refs/heads/main/security/1stdibs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Retail
- Marketplace
- Luxury Goods
- E-Commerce
- Furniture
- Art
- Jewelry
- MCP
---
