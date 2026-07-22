---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: craftcoffee.com
  spf: true
hosts:
- cert_expires: Sep 27 15:55:35 2026 GMT
  host: craftcoffee.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Craftcoffee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CraftCoffee, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CraftCoffee
provider_slug: craftcoffee
slug: craftcoffee-domain-security
source_filename: craftcoffee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: craftcoffee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 15:55:35 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: craftcoffee.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/craftcoffee/refs/heads/main/security/craftcoffee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Coffee
- Coffee Subscription
- Direct-to-Consumer
- E-Commerce
- Food and Beverage
- Subscription Commerce
- Retail
---
