---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bybe.com
  spf: true
hosts:
- cert_expires: Nov  8 23:59:59 2026 GMT
  host: bybe.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bybe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BYBE, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: BYBE
provider_slug: bybe
slug: bybe-domain-security
source_filename: bybe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bybe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: bybe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bybe/refs/heads/main/security/bybe-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Alcohol
- Beverages
- Promotions
- Rebates
- Marketing
- Retail
- CPG
---
