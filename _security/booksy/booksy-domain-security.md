---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: booksy.com
  spf: true
hosts:
- cert_expires: Feb  6 00:00:00 2027 GMT
  host: booksy.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: docs.booksy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  6 00:00:00 2027 GMT
  host: us.booksy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Booksy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Booksy, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Booksy
provider_slug: booksy
slug: booksy-domain-security
source_filename: booksy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: booksy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 00:00:00 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.booksy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: null\n- host: us.booksy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 00:00:00 2027 GMT\n  hsts: null\ndomains:\n- domain: booksy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/booksy/refs/heads/main/security/booksy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Beauty
- Wellness
- Booking
- Appointments
- Scheduling
- Marketplace
- Salons
- Barbershops
- Spas
- Payments
- Small Business
- Webhooks
---
