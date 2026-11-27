---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: canuckeats.com
  spf: true
hosts:
- cert_expires: Jan 18 08:17:33 2027 GMT
  host: canuckeats.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Canuck Eats Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Canuck Eats, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Canuck Eats
provider_slug: canuckeats-com
slug: canuckeats-com-domain-security
source_filename: canuckeats-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: canuckeats.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 08:17:33 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: canuckeats.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/canuckeats-com/security/canuckeats-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Food Delivery
- Canada
- Price Comparison
- Restaurant
- Marketplace
---
