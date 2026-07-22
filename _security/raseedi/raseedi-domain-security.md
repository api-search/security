---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: raseediapp.com
  spf: true
hosts:
- cert_expires: Sep  3 22:53:35 2026 GMT
  host: raseediapp.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Raseedi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Raseedi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Raseedi
provider_slug: raseedi
slug: raseedi-domain-security
source_filename: raseedi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: raseediapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 22:53:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: raseediapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/raseedi/refs/heads/main/security/raseedi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- FinTech
- Financial Services
- Mobile Payments
- Egypt
- Lending
- Telecom
- Financial Inclusion
---
