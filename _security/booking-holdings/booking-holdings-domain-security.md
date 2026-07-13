---
api_specs:
- filename: booking-com-demand-api.yaml
  format: yaml
  label: Booking.com Demand API
  slug: bookingcom-demand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-holdings/refs/heads/main/openapi/booking-com-demand-api.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bookingholdings.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: booking.com
  spf: true
hosts:
- cert_expires: Mar 26 23:59:59 2027 GMT
  host: www.bookingholdings.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 01:12:14 2026 GMT
  host: developers.booking.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: demandapi.booking.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Booking Holdings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Booking Holdings, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Booking Holdings
provider_slug: booking-holdings
slug: booking-holdings-domain-security
source_filename: booking-holdings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bookingholdings.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 26 23:59:59 2027 GMT\n  hsts: false\n- host: developers.booking.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 01:12:14 2026 GMT\n  hsts: false\n- host: demandapi.booking.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: bookingholdings.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: booking.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/booking-holdings/refs/heads/main/security/booking-holdings-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Accommodations
- Airlines
- Car Rentals
- Hospitality
- Hotels
- Restaurants
- Travel
---
