---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: finedinemenu.com
  spf: true
hosts:
- cert_expires: Aug 29 03:40:05 2026 GMT
  host: finedinemenu.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Finedine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FineDine, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: FineDine
provider_slug: finedine
slug: finedine-domain-security
source_filename: finedine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: finedinemenu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 03:40:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: finedinemenu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finedine/refs/heads/main/security/finedine-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Restaurants
- Hospitality
- Digital Menu
- Ordering
- Point of Sale
- Reservations
- Food and Beverage
- SaaS
---
