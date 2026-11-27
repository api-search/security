---
api_specs:
- filename: myplate-food-body-metrics-api-openapi.yml
  format: yaml
  label: MyPlate Body metrics API
  slug: myplate-food-body-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myplate-food/openapi/myplate-food-body-metrics-api-openapi.yml
- filename: myplate-food-energy-macros-api-openapi.yml
  format: yaml
  label: MyPlate Energy & macros API
  slug: myplate-food-energy-macros-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myplate-food/openapi/myplate-food-energy-macros-api-openapi.yml
- filename: myplate-food-guideline-tools-api-openapi.yml
  format: yaml
  label: MyPlate Guideline tools API
  slug: myplate-food-guideline-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myplate-food/openapi/myplate-food-guideline-tools-api-openapi.yml
- filename: myplate-food-meta-api-openapi.yml
  format: yaml
  label: MyPlate Meta API
  slug: myplate-food-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myplate-food/openapi/myplate-food-meta-api-openapi.yml
- filename: myplate-food-myplate-plan-api-openapi.yml
  format: yaml
  label: MyPlate MyPlate plan API
  slug: myplate-food-myplate-plan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myplate-food/openapi/myplate-food-myplate-plan-api-openapi.yml
- filename: myplate-food-recipes-api-openapi.yml
  format: yaml
  label: MyPlate Recipes API
  slug: myplate-food-recipes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myplate-food/openapi/myplate-food-recipes-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: myplate.food
  spf: true
hosts:
- cert_expires: Feb  7 18:42:50 2027 GMT
  host: myplate.food
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MyPlate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MyPlate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MyPlate
provider_slug: myplate-food
slug: myplate-food-domain-security
source_filename: myplate-food-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: myplate.food\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 18:42:50 2027 GMT\n  hsts: false\ndomains:\n- domain: myplate.food\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/myplate-food/security/myplate-food-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Food
- Nutrition
- USDA
- Calculator
- Recipes
---
