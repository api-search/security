---
api_specs:
- filename: lodgify-availability-api-openapi.yml
  format: yaml
  label: Lodgify Availability API
  slug: lodgify-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lodgify/refs/heads/main/openapi/lodgify-availability-api-openapi.yml
- filename: lodgify-bookings-api-openapi.yml
  format: yaml
  label: Lodgify Bookings API
  slug: lodgify-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lodgify/refs/heads/main/openapi/lodgify-bookings-api-openapi.yml
- filename: lodgify-messaging-api-openapi.yml
  format: yaml
  label: Lodgify Messaging API
  slug: lodgify-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lodgify/refs/heads/main/openapi/lodgify-messaging-api-openapi.yml
- filename: lodgify-properties-api-openapi.yml
  format: yaml
  label: Lodgify Properties API
  slug: lodgify-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lodgify/refs/heads/main/openapi/lodgify-properties-api-openapi.yml
- filename: lodgify-rates-quotes-api-openapi.yml
  format: yaml
  label: Lodgify Rates & Quotes API
  slug: lodgify-rates-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lodgify/refs/heads/main/openapi/lodgify-rates-quotes-api-openapi.yml
- filename: lodgify-webhooks-api-openapi.yml
  format: yaml
  label: Lodgify Webhooks API
  slug: lodgify-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lodgify/refs/heads/main/openapi/lodgify-webhooks-api-openapi.yml
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
