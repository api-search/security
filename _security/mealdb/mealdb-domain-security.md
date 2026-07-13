---
api_specs:
- filename: openapi.json
  format: json
  label: TheMealDB Recipe API
  slug: themealdb-recipe-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mealdb/refs/heads/main/openapi/openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: themealdb.com
  spf: false
hosts:
- cert_expires: Sep  8 01:51:06 2026 GMT
  host: www.themealdb.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mealdb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TheMealDB, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: TheMealDB
provider_slug: mealdb
slug: mealdb-domain-security
source_filename: mealdb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.themealdb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 01:51:06 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: themealdb.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mealdb/refs/heads/main/security/mealdb-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Food
- Recipes
- Meals
- Cooking
- Ingredients
- Cuisine
- Open Data
---
