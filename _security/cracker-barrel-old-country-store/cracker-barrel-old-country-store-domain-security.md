---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: crackerbarrel.com
  spf: true
hosts:
- cert_expires: Aug 23 09:27:25 2026 GMT
  host: www.crackerbarrel.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cracker Barrel Old Country Store Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cracker Barrel Old Country Store, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cracker Barrel Old Country Store
provider_slug: cracker-barrel-old-country-store
slug: cracker-barrel-old-country-store-domain-security
source_filename: cracker-barrel-old-country-store-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.crackerbarrel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 09:27:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: crackerbarrel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cracker-barrel-old-country-store/refs/heads/main/security/cracker-barrel-old-country-store-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Country Store
- Dining
- Family Dining
- Gift Shops
- Loyalty Programs
- Mobile Ordering
- Restaurants
- Retail
- Southern Cuisine
- Fortune 1000
---
