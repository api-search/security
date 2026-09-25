---
api_specs:
- filename: booking-com-demand-api-3-2-openapi.yml
  format: yaml
  label: Booking.com Demand API
  slug: booking-com-demand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-demand-api-3-2-openapi.yml
- filename: booking-com-connect-api-openapi.yml
  format: yaml
  label: Booking.com Connect API
  slug: booking-com-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-connect-api-openapi.yml
- filename: booking-com-status-api-openapi.yml
  format: yaml
  label: Booking.com Status API
  slug: booking-com-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-status-api-openapi.yml
- filename: booking-com-charges-api-openapi.yml
  format: yaml
  label: Booking.com Charges API
  slug: booking-com-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-charges-api-openapi.yml
- filename: booking-com-contacts-api-openapi.yml
  format: yaml
  label: Booking.com Contacts API
  slug: booking-com-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-contacts-api-openapi.yml
- filename: booking-com-contracting-api-openapi.yml
  format: yaml
  label: Booking.com Contracting API
  slug: booking-com-contracting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-contracting-api-openapi.yml
- filename: booking-com-facilities-api-openapi.yml
  format: yaml
  label: Booking.com Facilities API
  slug: booking-com-facilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-facilities-api-openapi.yml
- filename: booking-com-historical-reservations-api-openapi.yml
  format: yaml
  label: Booking.com Historical Reservations API
  slug: booking-com-historical-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-historical-reservations-api-openapi.yml
- filename: booking-com-payments-api-openapi.yml
  format: yaml
  label: Booking.com Payments API
  slug: booking-com-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-payments-api-openapi.yml
- filename: booking-com-payments-by-booking-onboarding-api-openapi.yml
  format: yaml
  label: Booking.com Payments by Booking Onboarding API
  slug: booking-com-payments-by-booking-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-payments-by-booking-onboarding-api-openapi.yml
- filename: booking-com-property-api-openapi.yml
  format: yaml
  label: Booking.com Property API
  slug: booking-com-property-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-property-api-openapi.yml
- filename: booking-com-property-health-api-openapi.yml
  format: yaml
  label: Booking.com Property Health API
  slug: booking-com-property-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-property-health-api-openapi.yml
- filename: booking-com-reconciliation-api-openapi.yml
  format: yaml
  label: Booking.com Reconciliation API
  slug: booking-com-reconciliation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-reconciliation-api-openapi.yml
- filename: booking-com-rooms-api-openapi.yml
  format: yaml
  label: Booking.com Rooms API
  slug: booking-com-rooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-rooms-api-openapi.yml
- filename: booking-com-valueadds-api-openapi.yml
  format: yaml
  label: Booking.com Value Adds Catalog API
  slug: booking-com-valueadds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-valueadds-api-openapi.yml
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
- cert_expires: Nov 19 00:13:51 2026 GMT
  host: developers.booking.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: demandapi.booking.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Booking Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Booking.com, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Booking.com
provider_slug: booking-com
slug: booking-com-domain-security
source_filename: booking-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.booking.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.booking.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 00:13:51 2026 GMT\n  hsts: false\n- host: demandapi.booking.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: booking.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/security/booking-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- Hospitality
- Accommodation
- Booking
- Car Rental
- Payments
- Connectivity
- Marketplace
- OTA
- Attractions
- A2A
---
