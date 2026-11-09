---
api_specs:
- filename: foodose-co-foods-api-openapi.yml
  format: yaml
  label: foodose Foods API
  slug: foodose-co-foods-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foodose-co/openapi/foodose-co-foods-api-openapi.yml
- filename: foodose-co-glp1-target-api-openapi.yml
  format: yaml
  label: foodose Glp1 Target API
  slug: foodose-co-glp1-target-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foodose-co/openapi/foodose-co-glp1-target-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: foodose.co
  spf: true
hosts:
- cert_expires: Feb  1 13:35:53 2027 GMT
  host: foodose.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Foodose Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for foodose, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: foodose
provider_slug: foodose-co
slug: foodose-co-domain-security
source_filename: foodose-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: foodose.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 13:35:53 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: foodose.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/foodose-co/security/foodose-co-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Health
- Nutrition
- GLP-1
- Calculator
- MealPlans
---
