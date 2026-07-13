---
api_specs:
- filename: edamam-recipe-search-v2-openapi.yml
  format: yaml
  label: Edamam Recipe Search API
  slug: edamam-recipe-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edamam-recipes/refs/heads/main/openapi/edamam-recipe-search-v2-openapi.yml
- filename: edamam-nutrition-analysis-v1-openapi.yml
  format: yaml
  label: Edamam Nutrition Analysis API
  slug: edamam-nutrition-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edamam-recipes/refs/heads/main/openapi/edamam-nutrition-analysis-v1-openapi.yml
- filename: edamam-food-database-v2-openapi.yml
  format: yaml
  label: Edamam Food Database API
  slug: edamam-food-database-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edamam-recipes/refs/heads/main/openapi/edamam-food-database-v2-openapi.yml
- filename: edamam-meal-planner-v1-openapi.yml
  format: yaml
  label: Edamam Meal Planner API
  slug: edamam-meal-planner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edamam-recipes/refs/heads/main/openapi/edamam-meal-planner-v1-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: edamam.com
  spf: true
hosts:
- cert_expires: Mar 31 10:34:31 2027 GMT
  host: www.edamam.com
  hsts: true
  hsts_max_age: 15552001
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 08:11:52 2026 GMT
  host: developer.edamam.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Mar 31 10:34:31 2027 GMT
  host: api.edamam.com
  hsts: true
  hsts_max_age: 15552001
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Edamam Recipes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Edamam, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Edamam
provider_slug: edamam-recipes
slug: edamam-recipes-domain-security
source_filename: edamam-recipes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.edamam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 31 10:34:31 2027 GMT\n  hsts: true\n  hsts_max_age: 15552001\n- host: developer.edamam.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  3 08:11:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.edamam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 31 10:34:31 2027 GMT\n  hsts: true\n  hsts_max_age: 15552001\ndomains:\n- domain: edamam.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edamam-recipes/refs/heads/main/security/edamam-recipes-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Food And Drink
- Recipes
- Nutrition
- Diet
- Allergens
- Meal Planning
- Sustainability
- Carbon Footprint
- Public APIs
---
