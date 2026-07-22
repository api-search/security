---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: getoze.com
  spf: true
hosts:
- cert_expires: Aug 20 07:51:19 2026 GMT
  host: getoze.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oze Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oze, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Oze
provider_slug: oze
slug: oze-domain-security
source_filename: oze-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getoze.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 07:51:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getoze.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oze/refs/heads/main/security/oze-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Fintech
- Small Business
- Bookkeeping
- Invoicing
- Lending
- Africa
- SME
---
