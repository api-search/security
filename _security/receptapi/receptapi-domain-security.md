---
api_specs:
- filename: receptapi-ingredients-api-openapi.yml
  format: yaml
  label: ReceptAPI Ingredients API
  slug: receptapi-ingredients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/receptapi/openapi/receptapi-ingredients-api-openapi.yml
- filename: receptapi-recipes-api-openapi.yml
  format: yaml
  label: ReceptAPI Recipes API
  slug: receptapi-recipes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/receptapi/openapi/receptapi-recipes-api-openapi.yml
- filename: receptapi-search-api-openapi.yml
  format: yaml
  label: ReceptAPI Search API
  slug: receptapi-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/receptapi/openapi/receptapi-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: receptapi.se
  spf: false
hosts:
- cert_expires: Jan 13 19:33:33 2027 GMT
  host: receptapi.se
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ReceptAPI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ReceptAPI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: ReceptAPI
provider_slug: receptapi
slug: receptapi-domain-security
source_filename: receptapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: receptapi.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 19:33:33 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: receptapi.se\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/receptapi/security/receptapi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Recipes
- Swedish
- Food
- Data
---
