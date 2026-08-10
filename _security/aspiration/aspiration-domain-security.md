---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: greenfi.com
  spf: true
hosts:
- cert_expires: Mar 19 23:59:59 2027 GMT
  host: www.greenfi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aspiration Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GreenFi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GreenFi
provider_slug: aspiration
slug: aspiration-domain-security
source_filename: aspiration-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.greenfi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: greenfi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aspiration/refs/heads/main/security/aspiration-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Banking
- Financial Services
- Fintech
- Consumer Banking
- Savings
- Investing
- Sustainability
- Climate
- Marketplace
---
