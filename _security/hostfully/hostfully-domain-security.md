---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hostfully.com
  spf: true
hosts:
- cert_expires: Sep 27 20:57:51 2026 GMT
  host: www.hostfully.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 14:40:07 2026 GMT
  host: dev.hostfully.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hostfully Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hostfully, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hostfully
provider_slug: hostfully
slug: hostfully-domain-security
source_filename: hostfully-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hostfully.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 20:57:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev.hostfully.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 14:40:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hostfully.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hostfully/refs/heads/main/security/hostfully-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Short-Term Rental
- Vacation Rental
- Property Management
- PMS
- Hospitality
- Channel Manager
- Direct Booking
- Real Estate
- Travel
- Booking
- Reservations
- Guest Communication
- Webhooks
- GraphQL
- OAuth 2.0
---
