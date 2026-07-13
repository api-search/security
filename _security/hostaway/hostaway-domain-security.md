---
api_specs:
- filename: hostaway-listings-api-openapi.yml
  format: yaml
  label: Hostaway Listings API
  slug: hostaway-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostaway/refs/heads/main/openapi/hostaway-listings-api-openapi.yml
- filename: hostaway-reservations-api-openapi.yml
  format: yaml
  label: Hostaway Reservations API
  slug: hostaway-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostaway/refs/heads/main/openapi/hostaway-reservations-api-openapi.yml
- filename: hostaway-calendar-api-openapi.yml
  format: yaml
  label: Hostaway Calendar API
  slug: hostaway-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostaway/refs/heads/main/openapi/hostaway-calendar-api-openapi.yml
- filename: hostaway-webhooks-api-openapi.yml
  format: yaml
  label: Hostaway Webhooks API
  slug: hostaway-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostaway/refs/heads/main/openapi/hostaway-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hostaway.com
  spf: true
hosts:
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: www.hostaway.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: api.hostaway.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hostaway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hostaway, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hostaway
provider_slug: hostaway
slug: hostaway-domain-security
source_filename: hostaway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hostaway.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.hostaway.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: hostaway.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hostaway/refs/heads/main/security/hostaway-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Vacation Rentals
- Short-Term Rentals
- Property Management
- Channel Manager
- Airbnb
- Vrbo
- Booking.com
- Expedia
- SaaS
---
