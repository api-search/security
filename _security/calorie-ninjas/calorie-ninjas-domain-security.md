---
api_specs:
- filename: calorieninjas-openapi.yml
  format: yaml
  label: CalorieNinjas API
  slug: calorieninjas
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calorie-ninjas/refs/heads/main/openapi/calorieninjas-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: calorieninjas.com
  spf: false
hosts:
- cert_expires: Nov  2 23:59:59 2026 GMT
  host: calorieninjas.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: api.calorieninjas.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Calorie Ninjas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CalorieNinjas, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: CalorieNinjas
provider_slug: calorie-ninjas
slug: calorie-ninjas-domain-security
source_filename: calorie-ninjas-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: calorieninjas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 23:59:59 2026 GMT\n  hsts: false\n- host: api.calorieninjas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: calorieninjas.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/calorie-ninjas/refs/heads/main/security/calorie-ninjas-domain-security.yml
summary_line: TLSv1.3
tags:
- Beverages
- Foods
- Image Recognition
- Nutrition
- Recipes
---
