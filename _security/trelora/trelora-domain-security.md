---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: trelora.com
  spf: true
hosts:
- cert_expires: Sep 17 15:46:17 2026 GMT
  host: trelora.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trelora Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trelora, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Trelora
provider_slug: trelora
slug: trelora-domain-security
source_filename: trelora-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trelora.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 15:46:17 2026 GMT\n  hsts: false\ndomains:\n- domain: trelora.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trelora/refs/heads/main/security/trelora-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Real Estate
- Real Estate Brokerage
- Home Buying
- Home Selling
- Real Estate Commissions
- Discount Brokerage
- IDX
- Property Search
---
