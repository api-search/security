---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: roofstock.com
  spf: true
hosts:
- cert_expires: Dec  4 20:04:22 2026 GMT
  host: www.roofstock.com
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Roofstock Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Roofstock, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Roofstock
provider_slug: roofstock
slug: roofstock-domain-security
source_filename: roofstock-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.roofstock.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 20:04:22 2026 GMT\n  hsts: true\n  hsts_max_age: 10886400\ndomains:\n- domain: roofstock.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roofstock/refs/heads/main/security/roofstock-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Real Estate
- PropTech
- Investing
- Single-Family Rentals
- Marketplace
- FinTech
---
