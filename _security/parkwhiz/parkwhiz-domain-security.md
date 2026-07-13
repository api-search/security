---
api_specs:
- filename: parkwhiz-openapi.yml
  format: yaml
  label: ParkWhiz Quotes & Locations API
  slug: parkwhiz-quotes-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parkwhiz/refs/heads/main/openapi/parkwhiz-openapi.yml
- filename: parkwhiz-openapi.yml
  format: yaml
  label: ParkWhiz Bookings API
  slug: parkwhiz-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parkwhiz/refs/heads/main/openapi/parkwhiz-openapi.yml
- filename: parkwhiz-openapi.yml
  format: yaml
  label: ParkWhiz Monthly Parking API
  slug: parkwhiz-monthly-parking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parkwhiz/refs/heads/main/openapi/parkwhiz-openapi.yml
- filename: parkwhiz-openapi.yml
  format: yaml
  label: ParkWhiz Venues & Events API
  slug: parkwhiz-venues-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parkwhiz/refs/heads/main/openapi/parkwhiz-openapi.yml
- filename: parkwhiz-openapi.yml
  format: yaml
  label: ParkWhiz Accounts & Vehicles API
  slug: parkwhiz-accounts-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parkwhiz/refs/heads/main/openapi/parkwhiz-openapi.yml
- filename: parkwhiz-openapi.yml
  format: yaml
  label: ParkWhiz Tickets API
  slug: parkwhiz-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parkwhiz/refs/heads/main/openapi/parkwhiz-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: parkwhiz.com
  spf: true
hosts:
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: www.parkwhiz.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: developer.parkwhiz.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: api.parkwhiz.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Parkwhiz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ParkWhiz, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ParkWhiz
provider_slug: parkwhiz
slug: parkwhiz-domain-security
source_filename: parkwhiz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.parkwhiz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.parkwhiz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: false\n- host: api.parkwhiz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: parkwhiz.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parkwhiz/refs/heads/main/security/parkwhiz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Parking
- Mobility
- Reservations
- Bookings
- Transportation
- Location
- Events
---
