---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: eatstreet.com
  spf: true
hosts:
- cert_expires: Mar 16 23:59:59 2027 GMT
  host: eatstreet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Eatstreet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EatStreet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: EatStreet
provider_slug: eatstreet
slug: eatstreet-domain-security
source_filename: eatstreet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eatstreet.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: eatstreet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eatstreet/refs/heads/main/security/eatstreet-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Food Delivery
- Restaurants
- Online Ordering
- Marketplace
- Local Commerce
- Consumer
- Point of Sale
- OAuth
---
