---
api_specs:
- filename: tripcom-searchattractionandactivity-api-openapi.yml
  format: yaml
  label: Trip.com SearchAttractionAndActivity API
  slug: tripcom-searchattractionandactivity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tripcom/refs/heads/main/openapi/tripcom-searchattractionandactivity-api-openapi.yml
- filename: tripcom-searchcars-api-openapi.yml
  format: yaml
  label: Trip.com SearchCars API
  slug: tripcom-searchcars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tripcom/refs/heads/main/openapi/tripcom-searchcars-api-openapi.yml
- filename: tripcom-searchflightticket-api-openapi.yml
  format: yaml
  label: Trip.com SearchFlightTicket API
  slug: tripcom-searchflightticket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tripcom/refs/heads/main/openapi/tripcom-searchflightticket-api-openapi.yml
- filename: tripcom-searchhotel-api-openapi.yml
  format: yaml
  label: Trip.com SearchHotel API
  slug: tripcom-searchhotel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tripcom/refs/heads/main/openapi/tripcom-searchhotel-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: trip.com
  spf: true
hosts:
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: www.trip.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tripcom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trip.com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Trip.com
provider_slug: tripcom
slug: tripcom-domain-security
source_filename: tripcom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: trip.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tripcom/refs/heads/main/security/tripcom-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Travel
- Hotels
- Flights
- Car Rental
- Attractions
- Trains
- Booking
- Itinerary
- AI Plugin
---
