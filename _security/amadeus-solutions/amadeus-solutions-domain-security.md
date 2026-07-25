---
api_specs:
- filename: amadeus-solutions-display-seatmaps-api-openapi.yml
  format: yaml
  label: Amadeus Solutions Display SeatMaps API
  slug: amadeus-solutions-display-seatmaps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/openapi/amadeus-solutions-display-seatmaps-api-openapi.yml
- filename: amadeus-solutions-shopping-api-openapi.yml
  format: yaml
  label: Amadeus Solutions Shopping API
  slug: amadeus-solutions-shopping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/openapi/amadeus-solutions-shopping-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: amadeus.com
  spf: true
hosts:
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: developers.amadeus.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  1 23:59:59 2026 GMT
  host: test.api.amadeus.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amadeus Solutions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amadeus Solutions, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
slug: amadeus-solutions-domain-security
source_filename: amadeus-solutions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.amadeus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: test.api.amadeus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: amadeus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/security/amadeus-solutions-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
---
