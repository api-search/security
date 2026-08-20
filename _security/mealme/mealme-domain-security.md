---
api_specs:
- filename: mealme-carts-api-openapi.yml
  format: yaml
  label: MealMe Carts API
  slug: mealme-carts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mealme/refs/heads/main/openapi/mealme-carts-api-openapi.yml
- filename: mealme-connect-accounts-api-openapi.yml
  format: yaml
  label: MealMe Connect Accounts API
  slug: mealme-connect-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mealme/refs/heads/main/openapi/mealme-connect-accounts-api-openapi.yml
- filename: mealme-geocoding-api-openapi.yml
  format: yaml
  label: MealMe Geocoding API
  slug: mealme-geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mealme/refs/heads/main/openapi/mealme-geocoding-api-openapi.yml
- filename: mealme-orders-api-openapi.yml
  format: yaml
  label: MealMe Orders API
  slug: mealme-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mealme/refs/heads/main/openapi/mealme-orders-api-openapi.yml
- filename: mealme-payments-api-openapi.yml
  format: yaml
  label: MealMe Payments API
  slug: mealme-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mealme/refs/heads/main/openapi/mealme-payments-api-openapi.yml
- filename: mealme-search-api-openapi.yml
  format: yaml
  label: MealMe Search API
  slug: mealme-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mealme/refs/heads/main/openapi/mealme-search-api-openapi.yml
- filename: mealme-stores-api-openapi.yml
  format: yaml
  label: MealMe Stores API
  slug: mealme-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mealme/refs/heads/main/openapi/mealme-stores-api-openapi.yml
- filename: mealme-support-chat-api-openapi.yml
  format: yaml
  label: MealMe Support Chat API
  slug: mealme-support-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mealme/refs/heads/main/openapi/mealme-support-chat-api-openapi.yml
- filename: mealme-tracking-api-openapi.yml
  format: yaml
  label: MealMe Tracking API
  slug: mealme-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mealme/refs/heads/main/openapi/mealme-tracking-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mealme.ai
  spf: true
hosts:
- cert_expires: Aug 15 13:22:20 2026 GMT
  host: www.mealme.ai
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 24 23:59:59 2026 GMT
  host: api.mealme.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mealme Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MealMe, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MealMe
provider_slug: mealme
slug: mealme-domain-security
source_filename: mealme-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mealme.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 13:22:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: api.mealme.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: mealme.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mealme/refs/heads/main/security/mealme-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Delivery
- Food
- Grocery
- Ordering
- Restaurant
---
