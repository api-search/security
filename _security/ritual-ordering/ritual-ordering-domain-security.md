---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ritual.co
  spf: true
hosts:
- cert_expires: Sep 16 08:25:57 2026 GMT
  host: ritual.co
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ritual Ordering Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ritual, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Ritual
provider_slug: ritual-ordering
slug: ritual-ordering-domain-security
source_filename: ritual-ordering-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ritual.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 08:25:57 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: ritual.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ritual-ordering/refs/heads/main/security/ritual-ordering-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Restaurants
- Order Ahead
- Online Ordering
- Food Ordering
- Social Ordering
- Payments
- POS Integration
- No Public API
---
