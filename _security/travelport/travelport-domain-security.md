---
api_specs:
- filename: travelport-booking-api-openapi.yml
  format: yaml
  label: Travelport Booking API
  slug: travelport-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelport/refs/heads/main/openapi/travelport-booking-api-openapi.yml
- filename: travelport-emds-api-openapi.yml
  format: yaml
  label: Travelport EMDs API
  slug: travelport-emds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelport/refs/heads/main/openapi/travelport-emds-api-openapi.yml
- filename: travelport-fare-rules-api-openapi.yml
  format: yaml
  label: Travelport Fare Rules API
  slug: travelport-fare-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelport/refs/heads/main/openapi/travelport-fare-rules-api-openapi.yml
- filename: travelport-modifications-api-openapi.yml
  format: yaml
  label: Travelport Modifications API
  slug: travelport-modifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelport/refs/heads/main/openapi/travelport-modifications-api-openapi.yml
- filename: travelport-pricing-api-openapi.yml
  format: yaml
  label: Travelport Pricing API
  slug: travelport-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelport/refs/heads/main/openapi/travelport-pricing-api-openapi.yml
- filename: travelport-queues-api-openapi.yml
  format: yaml
  label: Travelport Queues API
  slug: travelport-queues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelport/refs/heads/main/openapi/travelport-queues-api-openapi.yml
- filename: travelport-reservations-api-openapi.yml
  format: yaml
  label: Travelport Reservations API
  slug: travelport-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelport/refs/heads/main/openapi/travelport-reservations-api-openapi.yml
- filename: travelport-search-api-openapi.yml
  format: yaml
  label: Travelport Search API
  slug: travelport-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelport/refs/heads/main/openapi/travelport-search-api-openapi.yml
- filename: travelport-seats-and-ancillaries-api-openapi.yml
  format: yaml
  label: Travelport Seats and Ancillaries API
  slug: travelport-seats-and-ancillaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelport/refs/heads/main/openapi/travelport-seats-and-ancillaries-api-openapi.yml
- filename: travelport-ticketing-api-openapi.yml
  format: yaml
  label: Travelport Ticketing API
  slug: travelport-ticketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelport/refs/heads/main/openapi/travelport-ticketing-api-openapi.yml
- filename: travelport-workbench-api-openapi.yml
  format: yaml
  label: Travelport Workbench API
  slug: travelport-workbench-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelport/refs/heads/main/openapi/travelport-workbench-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: travelport.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: travelport.net
  spf: false
hosts:
- cert_expires: Aug 29 06:23:43 2026 GMT
  host: www.travelport.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 11:02:52 2026 GMT
  host: developer.travelport.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 22 23:59:59 2026 GMT
  host: api.travelport.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Travelport Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Travelport, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Travelport
provider_slug: travelport
slug: travelport-domain-security
source_filename: travelport-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.travelport.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 06:23:43 2026 GMT\n  hsts: false\n- host: developer.travelport.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 11:02:52 2026 GMT\n  hsts: false\n- host: api.travelport.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: travelport.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: travelport.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/travelport/refs/heads/main/security/travelport-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Travel
- Travel Technology
- Reservations
- GDS
- NDC
- Flights
- Hotels
- Payments
---
