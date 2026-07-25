---
api_specs:
- filename: themealdb-filter-api-openapi.yml
  format: yaml
  label: TheMealDB Filter API
  slug: themealdb-filter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/themealdb/refs/heads/main/openapi/themealdb-filter-api-openapi.yml
- filename: themealdb-list-api-openapi.yml
  format: yaml
  label: TheMealDB List API
  slug: themealdb-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/themealdb/refs/heads/main/openapi/themealdb-list-api-openapi.yml
- filename: themealdb-lookup-api-openapi.yml
  format: yaml
  label: TheMealDB Lookup API
  slug: themealdb-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/themealdb/refs/heads/main/openapi/themealdb-lookup-api-openapi.yml
- filename: themealdb-search-api-openapi.yml
  format: yaml
  label: TheMealDB Search API
  slug: themealdb-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/themealdb/refs/heads/main/openapi/themealdb-search-api-openapi.yml
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
name: Themealdb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TheMealDB, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: TheMealDB
provider_slug: themealdb
slug: themealdb-domain-security
source_filename: themealdb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.themealdb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 01:51:06 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: themealdb.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/themealdb/refs/heads/main/security/themealdb-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Recipes
- Meals
- Food
- Cooking
---
