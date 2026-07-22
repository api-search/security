---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: caterwings.de
  spf: true
hosts:
- cert_expires: Aug 30 01:55:41 2026 GMT
  host: caterwings.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Caterwings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Caterwings, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Caterwings
provider_slug: caterwings
slug: caterwings-domain-security
source_filename: caterwings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: caterwings.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 01:55:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: caterwings.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caterwings/refs/heads/main/security/caterwings-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Consumer
- Marketplace
- Catering
- Food Delivery
- Food and Beverage
- Europe
- Defunct
---
