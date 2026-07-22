---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: touramigo.com
  spf: true
hosts:
- cert_expires: Sep 17 15:33:56 2026 GMT
  host: touramigo.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 15:33:56 2026 GMT
  host: www.touramigo.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 14 23:59:59 2027 GMT
  host: api.touramigo.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Touramigo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TourAmigo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TourAmigo
provider_slug: touramigo
slug: touramigo-domain-security
source_filename: touramigo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: touramigo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 15:33:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: www.touramigo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 15:33:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: api.touramigo.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 14 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: touramigo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/touramigo/refs/heads/main/security/touramigo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- Tours
- Booking
- Tour Operators
- Cruises
- Destination Management
- Channel Manager
- SaaS
---
