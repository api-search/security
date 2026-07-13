---
api_specs:
- filename: bookingcom-booking-api-openapi.yml
  format: yaml
  label: Booking.com API
  slug: booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bookingcom/refs/heads/main/openapi/bookingcom-booking-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: booking.com
  spf: true
hosts:
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: www.booking.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 01:12:14 2026 GMT
  host: developers.booking.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 23:59:59 2026 GMT
  host: api.booking.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bookingcom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Booking.com, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Booking.com
provider_slug: bookingcom
slug: bookingcom-domain-security
source_filename: bookingcom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.booking.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.booking.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 01:12:14 2026 GMT\n  hsts: false\n- host: api.booking.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: booking.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bookingcom/refs/heads/main/security/bookingcom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Accommodations
- Affiliates
- Connectivity
- Hospitality
- Hotels
- Reservations
- Travel
---
