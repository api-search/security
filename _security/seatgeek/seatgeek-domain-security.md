---
api_specs:
- filename: seatgeek-events-api-openapi.yml
  format: yaml
  label: SeatGeek Events API
  slug: seatgeek-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seatgeek/refs/heads/main/openapi/seatgeek-events-api-openapi.yml
- filename: seatgeek-performers-api-openapi.yml
  format: yaml
  label: SeatGeek Performers API
  slug: seatgeek-performers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seatgeek/refs/heads/main/openapi/seatgeek-performers-api-openapi.yml
- filename: seatgeek-recommendations-api-openapi.yml
  format: yaml
  label: SeatGeek Recommendations API
  slug: seatgeek-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seatgeek/refs/heads/main/openapi/seatgeek-recommendations-api-openapi.yml
- filename: seatgeek-taxonomies-api-openapi.yml
  format: yaml
  label: SeatGeek Taxonomies API
  slug: seatgeek-taxonomies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seatgeek/refs/heads/main/openapi/seatgeek-taxonomies-api-openapi.yml
- filename: seatgeek-venues-api-openapi.yml
  format: yaml
  label: SeatGeek Venues API
  slug: seatgeek-venues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seatgeek/refs/heads/main/openapi/seatgeek-venues-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: seatgeek.com
  spf: true
hosts:
- cert_expires: Oct  8 09:27:43 2026 GMT
  host: seatgeek.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 09:27:43 2026 GMT
  host: api.seatgeek.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Seatgeek Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SeatGeek, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SeatGeek
provider_slug: seatgeek
slug: seatgeek-domain-security
source_filename: seatgeek-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: seatgeek.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 09:27:43 2026 GMT\n  hsts: null\n- host: api.seatgeek.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 09:27:43 2026 GMT\n  hsts: null\ndomains:\n- domain: seatgeek.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seatgeek/refs/heads/main/security/seatgeek-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Events
- Tickets
- Live Events
- Concerts
- Sports
- Venues
- Ticketing
---
