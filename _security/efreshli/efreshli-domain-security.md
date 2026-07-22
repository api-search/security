---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: efreshli.com
  spf: true
hosts:
- cert_expires: Oct 13 10:02:10 2026 GMT
  host: efreshli.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Efreshli Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Efreshli, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Efreshli
provider_slug: efreshli
slug: efreshli-domain-security
source_filename: efreshli-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: efreshli.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 10:02:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: efreshli.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/efreshli/refs/heads/main/security/efreshli-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- E-commerce
- Furniture
- Home Furnishing
- Interior Design
- Retail
- AI
- Egypt
---
