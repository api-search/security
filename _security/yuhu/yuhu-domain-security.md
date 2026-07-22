---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: yuhu.io
  spf: true
hosts:
- cert_expires: Aug 24 09:26:08 2026 GMT
  host: developer.yuhu.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: api.yuhu.io
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Yuhu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yuhu, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Yuhu
provider_slug: yuhu
slug: yuhu-domain-security
source_filename: yuhu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.yuhu.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 09:26:08 2026 GMT\n  hsts: false\n- host: api.yuhu.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: yuhu.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yuhu/refs/heads/main/security/yuhu-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Property Management
- PropTech
- Real Estate
- Multifamily
- Rental
- Leasing
- Payments
- Partners API
---
