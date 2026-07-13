---
api_specs:
- filename: lodgify-openapi.yml
  format: yaml
  label: Lodgify Properties API
  slug: properties
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lodgify/refs/heads/main/openapi/lodgify-openapi.yml
- filename: lodgify-openapi.yml
  format: yaml
  label: Lodgify Rates & Availability API
  slug: rates-availability
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lodgify/refs/heads/main/openapi/lodgify-openapi.yml
- filename: lodgify-openapi.yml
  format: yaml
  label: Lodgify Bookings & Reservations API
  slug: bookings-reservations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lodgify/refs/heads/main/openapi/lodgify-openapi.yml
- filename: lodgify-openapi.yml
  format: yaml
  label: Lodgify Quotes API
  slug: quotes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lodgify/refs/heads/main/openapi/lodgify-openapi.yml
- filename: lodgify-openapi.yml
  format: yaml
  label: Lodgify Messaging API
  slug: messaging
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lodgify/refs/heads/main/openapi/lodgify-openapi.yml
- filename: lodgify-openapi.yml
  format: yaml
  label: Lodgify Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lodgify/refs/heads/main/openapi/lodgify-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: lodgify.com
  spf: true
hosts:
- cert_expires: Jan 13 16:57:37 2027 GMT
  host: www.lodgify.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 04:48:09 2026 GMT
  host: docs.lodgify.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 13 16:57:37 2027 GMT
  host: api.lodgify.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lodgify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lodgify, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Lodgify
provider_slug: lodgify
slug: lodgify-domain-security
source_filename: lodgify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lodgify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 16:57:37 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.lodgify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 04:48:09 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.lodgify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 16:57:37 2027 GMT\n  hsts: null\ndomains:\n- domain: lodgify.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lodgify/refs/heads/main/security/lodgify-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Vacation Rental
- Property Management
- Booking
- Channel Manager
- Travel
---
