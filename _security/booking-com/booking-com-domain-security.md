---
api_specs:
- filename: booking-com-demand-api-openapi.yml
  format: yaml
  label: Booking.com Demand API
  slug: demand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-demand-api-openapi.yml
- filename: booking-com-car-rentals-api-openapi.yml
  format: yaml
  label: Booking.com Car Rentals API
  slug: car-rentals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-car-rentals-api-openapi.yml
- filename: booking-com-connectivity-content-api-openapi.yml
  format: yaml
  label: Booking.com Connectivity Content API
  slug: connectivity-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-connectivity-content-api-openapi.yml
- filename: booking-com-connectivity-reservations-api-openapi.yml
  format: yaml
  label: Booking.com Connectivity Reservations API
  slug: connectivity-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-connectivity-reservations-api-openapi.yml
- filename: booking-com-connectivity-rates-availability-api-openapi.yml
  format: yaml
  label: Booking.com Connectivity Rates and Availability API
  slug: connectivity-rates-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-connectivity-rates-availability-api-openapi.yml
- filename: booking-com-connectivity-promotions-api-openapi.yml
  format: yaml
  label: Booking.com Connectivity Promotions API
  slug: connectivity-promotions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-connectivity-promotions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: booking.com
  spf: true
hosts:
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
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: supply-xml.booking.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Booking Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for booking-com, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: booking-com
provider_slug: booking-com
slug: booking-com-domain-security
source_filename: booking-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.booking.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 01:12:14 2026 GMT\n  hsts: false\n- host: demandapi.booking.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: null\n- host: supply-xml.booking.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: booking.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/security/booking-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags: []
---
