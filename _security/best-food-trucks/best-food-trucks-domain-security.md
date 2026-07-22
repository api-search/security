---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bestfoodtrucks.com
  spf: true
hosts:
- cert_expires: Aug 19 22:20:14 2026 GMT
  host: bestfoodtrucks.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Best Food Trucks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Best Food Trucks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Best Food Trucks
provider_slug: best-food-trucks
slug: best-food-trucks-domain-security
source_filename: best-food-trucks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bestfoodtrucks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 22:20:14 2026 GMT\n  hsts: null\ndomains:\n- domain: bestfoodtrucks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/best-food-trucks/refs/heads/main/security/best-food-trucks-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Food Trucks
- Food and Beverage
- Mobile Ordering
- Events
- Catering
- Point of Sale
---
