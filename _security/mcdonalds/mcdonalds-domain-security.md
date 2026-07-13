---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mcdonalds.com
  spf: true
hosts:
- cert_expires: Oct  8 13:24:25 2026 GMT
  host: www.mcdonalds.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 13:24:25 2026 GMT
  host: corporate.mcdonalds.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mcdonalds Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for McDonald''s, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: McDonald's
provider_slug: mcdonalds
slug: mcdonalds-domain-security
source_filename: mcdonalds-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mcdonalds.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 13:24:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: corporate.mcdonalds.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 13:24:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: mcdonalds.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mcdonalds/refs/heads/main/security/mcdonalds-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Delivery
- Fast Food
- Loyalty
- Mobile Ordering
- Ordering
- Restaurants
- Fortune 500
---
