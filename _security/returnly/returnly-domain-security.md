---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: returnly.com
  spf: true
hosts:
- cert_expires: Oct  2 03:58:01 2026 GMT
  host: returnly.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Returnly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Returnly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Returnly
provider_slug: returnly
slug: returnly-domain-security
source_filename: returnly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: returnly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 03:58:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: returnly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/returnly/refs/heads/main/security/returnly-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Fintech
- E-commerce
- Returns
- Exchanges
- Payments
- Acquired
---
