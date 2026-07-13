---
api_specs:
- filename: tickettailor-openapi.yml
  format: yaml
  label: Ticket Tailor Events API
  slug: tickettailor-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tickettailor/refs/heads/main/openapi/tickettailor-openapi.yml
- filename: tickettailor-openapi.yml
  format: yaml
  label: Ticket Tailor Event Series API
  slug: tickettailor-event-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tickettailor/refs/heads/main/openapi/tickettailor-openapi.yml
- filename: tickettailor-openapi.yml
  format: yaml
  label: Ticket Tailor Orders API
  slug: tickettailor-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tickettailor/refs/heads/main/openapi/tickettailor-openapi.yml
- filename: tickettailor-openapi.yml
  format: yaml
  label: Ticket Tailor Issued Tickets API
  slug: tickettailor-issued-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tickettailor/refs/heads/main/openapi/tickettailor-openapi.yml
- filename: tickettailor-openapi.yml
  format: yaml
  label: Ticket Tailor Vouchers API
  slug: tickettailor-vouchers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tickettailor/refs/heads/main/openapi/tickettailor-openapi.yml
- filename: tickettailor-openapi.yml
  format: yaml
  label: Ticket Tailor Check-ins API
  slug: tickettailor-check-ins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tickettailor/refs/heads/main/openapi/tickettailor-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tickettailor.com
  spf: true
hosts:
- cert_expires: Sep  8 22:49:35 2026 GMT
  host: www.tickettailor.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 19:55:44 2026 GMT
  host: developers.tickettailor.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 22:49:35 2026 GMT
  host: api.tickettailor.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tickettailor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ticket Tailor, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ticket Tailor
provider_slug: tickettailor
slug: tickettailor-domain-security
source_filename: tickettailor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tickettailor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 22:49:35 2026 GMT\n  hsts: null\n- host: developers.tickettailor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 19:55:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.tickettailor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 22:49:35 2026 GMT\n  hsts: null\ndomains:\n- domain: tickettailor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tickettailor/refs/heads/main/security/tickettailor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Event Ticketing
- Events
- Ticketing
- Box Office
- Payments
- Registration
---
