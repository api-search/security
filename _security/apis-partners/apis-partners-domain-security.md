---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: apis.pe
  spf: true
hosts:
- cert_expires: Sep 25 17:30:27 2026 GMT
  host: apis.pe
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Apis Partners Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apis Partners, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Apis Partners
provider_slug: apis-partners
slug: apis-partners-domain-security
source_filename: apis-partners-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apis.pe\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 25 17:30:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: apis.pe\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apis-partners/refs/heads/main/security/apis-partners-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Venture
- Private Equity
- Fintech
- Financial Services
- Payments
- Investor
- Emerging Markets
---
