---
api_specs:
- filename: spoton-availability-api-openapi.yml
  format: yaml
  label: SpotOn Availability API
  slug: spoton-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoton/refs/heads/main/openapi/spoton-availability-api-openapi.yml
- filename: spoton-cash-deposits-api-openapi.yml
  format: yaml
  label: SpotOn Cash Deposits API
  slug: spoton-cash-deposits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoton/refs/heads/main/openapi/spoton-cash-deposits-api-openapi.yml
- filename: spoton-employees-api-openapi.yml
  format: yaml
  label: SpotOn Employees API
  slug: spoton-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoton/refs/heads/main/openapi/spoton-employees-api-openapi.yml
- filename: spoton-job-positions-api-openapi.yml
  format: yaml
  label: SpotOn Job Positions API
  slug: spoton-job-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoton/refs/heads/main/openapi/spoton-job-positions-api-openapi.yml
- filename: spoton-locations-api-openapi.yml
  format: yaml
  label: SpotOn Locations API
  slug: spoton-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoton/refs/heads/main/openapi/spoton-locations-api-openapi.yml
- filename: spoton-menu-items-api-openapi.yml
  format: yaml
  label: SpotOn Menu Items API
  slug: spoton-menu-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoton/refs/heads/main/openapi/spoton-menu-items-api-openapi.yml
- filename: spoton-order-types-api-openapi.yml
  format: yaml
  label: SpotOn Order Types API
  slug: spoton-order-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoton/refs/heads/main/openapi/spoton-order-types-api-openapi.yml
- filename: spoton-orders-api-openapi.yml
  format: yaml
  label: SpotOn Orders API
  slug: spoton-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoton/refs/heads/main/openapi/spoton-orders-api-openapi.yml
- filename: spoton-paid-in-outs-api-openapi.yml
  format: yaml
  label: SpotOn Paid In Outs API
  slug: spoton-paid-in-outs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoton/refs/heads/main/openapi/spoton-paid-in-outs-api-openapi.yml
- filename: spoton-payment-options-api-openapi.yml
  format: yaml
  label: SpotOn Payment Options API
  slug: spoton-payment-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoton/refs/heads/main/openapi/spoton-payment-options-api-openapi.yml
- filename: spoton-report-categories-api-openapi.yml
  format: yaml
  label: SpotOn Report Categories API
  slug: spoton-report-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoton/refs/heads/main/openapi/spoton-report-categories-api-openapi.yml
- filename: spoton-reservations-api-openapi.yml
  format: yaml
  label: SpotOn Reservations API
  slug: spoton-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoton/refs/heads/main/openapi/spoton-reservations-api-openapi.yml
- filename: spoton-restaurants-api-openapi.yml
  format: yaml
  label: SpotOn Restaurants API
  slug: spoton-restaurants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoton/refs/heads/main/openapi/spoton-restaurants-api-openapi.yml
- filename: spoton-time-clock-entries-api-openapi.yml
  format: yaml
  label: SpotOn Time Clock Entries API
  slug: spoton-time-clock-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoton/refs/heads/main/openapi/spoton-time-clock-entries-api-openapi.yml
- filename: spoton-waitlist-api-openapi.yml
  format: yaml
  label: SpotOn Waitlist API
  slug: spoton-waitlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoton/refs/heads/main/openapi/spoton-waitlist-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: spoton.com
  spf: true
hosts:
- cert_expires: Oct  9 08:35:21 2026 GMT
  host: www.spoton.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 00:11:09 2026 GMT
  host: developers.spoton.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 10 23:59:59 2027 GMT
  host: restaurantapi.spoton.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spoton Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SpotOn, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SpotOn
provider_slug: spoton
slug: spoton-domain-security
source_filename: spoton-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.spoton.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 08:35:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.spoton.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 00:11:09 2026 GMT\n  hsts: null\n- host: restaurantapi.spoton.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: spoton.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spoton/refs/heads/main/security/spoton-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Restaurant
- Point of Sale
- Payments
- Online Ordering
- Reservations
- Reporting
---
