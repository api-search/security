---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: crossave.com
  spf: true
hosts:
- cert_expires: Dec 13 09:04:21 2026 GMT
  host: crossave.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Crossave Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crossave, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Crossave
provider_slug: crossave-com
slug: crossave-com-domain-security
source_filename: crossave-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crossave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 09:04:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: crossave.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/crossave-com/security/crossave-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- E-Commerce
- Collectibles
- Price Comparison
- import-duty
- International Shipping
---
