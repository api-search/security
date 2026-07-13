---
api_specs:
- filename: mealme-openapi.yml
  format: yaml
  label: MealMe Food Ordering API
  slug: mealme-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mealme/refs/heads/main/openapi/mealme-openapi.yml
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
- Restaurants
---
