---
api_specs:
- filename: whiplash-bundle-items-api-openapi.yml
  format: yaml
  label: Whiplash Bundle Items API
  slug: whiplash-bundle-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whiplash/refs/heads/main/openapi/whiplash-bundle-items-api-openapi.yml
- filename: whiplash-consumer-returns-api-openapi.yml
  format: yaml
  label: Whiplash Consumer Returns API
  slug: whiplash-consumer-returns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whiplash/refs/heads/main/openapi/whiplash-consumer-returns-api-openapi.yml
- filename: whiplash-customers-api-openapi.yml
  format: yaml
  label: Whiplash Customers API
  slug: whiplash-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whiplash/refs/heads/main/openapi/whiplash-customers-api-openapi.yml
- filename: whiplash-documents-api-openapi.yml
  format: yaml
  label: Whiplash Documents API
  slug: whiplash-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whiplash/refs/heads/main/openapi/whiplash-documents-api-openapi.yml
- filename: whiplash-items-api-openapi.yml
  format: yaml
  label: Whiplash Items API
  slug: whiplash-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whiplash/refs/heads/main/openapi/whiplash-items-api-openapi.yml
- filename: whiplash-notification-events-api-openapi.yml
  format: yaml
  label: Whiplash Notification Events API
  slug: whiplash-notification-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whiplash/refs/heads/main/openapi/whiplash-notification-events-api-openapi.yml
- filename: whiplash-notification-subscriptions-api-openapi.yml
  format: yaml
  label: Whiplash Notification Subscriptions API
  slug: whiplash-notification-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whiplash/refs/heads/main/openapi/whiplash-notification-subscriptions-api-openapi.yml
- filename: whiplash-orders-api-openapi.yml
  format: yaml
  label: Whiplash Orders API
  slug: whiplash-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whiplash/refs/heads/main/openapi/whiplash-orders-api-openapi.yml
- filename: whiplash-shipnotices-api-openapi.yml
  format: yaml
  label: Whiplash Shipnotices API
  slug: whiplash-shipnotices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whiplash/refs/heads/main/openapi/whiplash-shipnotices-api-openapi.yml
- filename: whiplash-simulate-api-openapi.yml
  format: yaml
  label: Whiplash Simulate API
  slug: whiplash-simulate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whiplash/refs/heads/main/openapi/whiplash-simulate-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getwhiplash.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: whiplash.com
  spf: true
hosts:
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: www.getwhiplash.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep  9 16:20:50 2026 GMT
  host: help.whiplash.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
- host: api.getwhiplash.com
  https: false
kind: domain-security
layout: security
method: probed
name: Whiplash Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Whiplash, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Whiplash
provider_slug: whiplash
slug: whiplash-domain-security
source_filename: whiplash-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getwhiplash.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: false\n- host: help.whiplash.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 16:20:50 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: api.getwhiplash.com\n  https: false\ndomains:\n- domain: getwhiplash.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n- domain: whiplash.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whiplash/refs/heads/main/security/whiplash-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Fulfillment
- 3PL
- Logistics
- Ecommerce
- Orders
- Inventory
- Shipments
- Returns
- Warehousing
---
