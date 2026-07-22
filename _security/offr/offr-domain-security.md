---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: offr.io
  spf: true
hosts:
- cert_expires: Mar  1 23:59:59 2027 GMT
  host: offr.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Offr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Offr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Offr
provider_slug: offr
slug: offr-domain-security
source_filename: offr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: offr.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: offr.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/offr/refs/heads/main/security/offr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- PropTech
- Real Estate
- Property Transactions
- Auctions
- Lettings
- Offer Management
- Ireland
---
