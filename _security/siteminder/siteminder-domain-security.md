---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: siteminder.com
  spf: true
hosts:
- cert_expires: Sep  5 18:10:04 2026 GMT
  host: developer.siteminder.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Siteminder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SiteMinder, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SiteMinder
provider_slug: siteminder
slug: siteminder-domain-security
source_filename: siteminder-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.siteminder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 18:10:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: siteminder.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/siteminder/refs/heads/main/security/siteminder-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Hospitality
- Hotel Distribution
- Channel Manager
- Booking Engine
- Travel
- Property Management
- Reservations
---
