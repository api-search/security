---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: stockeld.com
  spf: true
hosts:
- cert_expires: Sep 13 04:12:33 2026 GMT
  host: www.stockeld.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stockeld Dreamery Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stockeld Dreamery, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Stockeld Dreamery
provider_slug: stockeld-dreamery
slug: stockeld-dreamery-domain-security
source_filename: stockeld-dreamery-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stockeld.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 04:12:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: stockeld.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stockeld-dreamery/refs/heads/main/security/stockeld-dreamery-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Food Tech
- Plant-Based
- Sustainability
- CPG
- Foodservice
- Sweden
---
