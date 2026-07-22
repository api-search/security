---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bloominbrands.com
  spf: true
hosts:
- cert_expires: Aug  9 10:37:38 2026 GMT
  host: www.bloominbrands.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bloomin Brands Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bloomin'' Brands, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bloomin' Brands
provider_slug: bloomin-brands
slug: bloomin-brands-domain-security
source_filename: bloomin-brands-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bloominbrands.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  9 10:37:38 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: bloominbrands.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomin-brands/refs/heads/main/security/bloomin-brands-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Restaurants
- Dining
- Hospitality
- Loyalty
- Food
- Casual Dining
- Online Ordering
- Mobile Apps
---
