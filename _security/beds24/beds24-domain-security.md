---
api_specs:
- filename: beds24-openapi.yml
  format: yaml
  label: Beds24 Authentication API
  slug: beds24-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beds24/refs/heads/main/openapi/beds24-openapi.yml
- filename: beds24-openapi.yml
  format: yaml
  label: Beds24 Bookings API
  slug: beds24-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beds24/refs/heads/main/openapi/beds24-openapi.yml
- filename: beds24-openapi.yml
  format: yaml
  label: Beds24 Invoices & Charges API
  slug: beds24-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beds24/refs/heads/main/openapi/beds24-openapi.yml
- filename: beds24-openapi.yml
  format: yaml
  label: Beds24 Booking Messages API
  slug: beds24-booking-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beds24/refs/heads/main/openapi/beds24-openapi.yml
- filename: beds24-openapi.yml
  format: yaml
  label: Beds24 Properties API
  slug: beds24-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beds24/refs/heads/main/openapi/beds24-openapi.yml
- filename: beds24-openapi.yml
  format: yaml
  label: Beds24 Availability & Calendar API
  slug: beds24-availability-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beds24/refs/heads/main/openapi/beds24-openapi.yml
- filename: beds24-openapi.yml
  format: yaml
  label: Beds24 Rates & Prices API
  slug: beds24-rates-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beds24/refs/heads/main/openapi/beds24-openapi.yml
- filename: beds24-openapi.yml
  format: yaml
  label: Beds24 Channels API
  slug: beds24-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beds24/refs/heads/main/openapi/beds24-openapi.yml
- filename: beds24-openapi.yml
  format: yaml
  label: Beds24 Accounts API
  slug: beds24-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beds24/refs/heads/main/openapi/beds24-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: beds24.com
  spf: true
hosts:
- cert_expires: Oct 11 23:59:59 2026 GMT
  host: beds24.com
  hsts: true
  hsts_max_age: 31415926
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  4 22:26:31 2026 GMT
  host: wiki.beds24.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 23:59:59 2026 GMT
  host: api.beds24.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Beds24 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beds24, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Beds24
provider_slug: beds24
slug: beds24-domain-security
source_filename: beds24-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: beds24.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31415926\n- host: wiki.beds24.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 22:26:31 2026 GMT\n  hsts: false\n- host: api.beds24.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 11 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: beds24.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beds24/refs/heads/main/security/beds24-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Vacation Rental
- Hotel
- Channel Manager
- Property Management System
- Booking Engine
- Hospitality
- Reservations
---
