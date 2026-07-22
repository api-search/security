---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: partender.com
  spf: true
hosts:
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: app.partender.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Partender Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Partender, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Partender
provider_slug: partender
slug: partender-domain-security
source_filename: partender-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: app.partender.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: partender.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/partender/refs/heads/main/security/partender-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Bar Inventory
- Hospitality
- Restaurants
- Inventory Management
- Beverage
- Point of Sale
- Ordering
---
