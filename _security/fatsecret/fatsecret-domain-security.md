---
api_specs:
- filename: fatsecret-exercise-diary-api-openapi.yml
  format: yaml
  label: fatsecret Exercise Diary API
  slug: fatsecret-exercise-diary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-exercise-diary-api-openapi.yml
- filename: fatsecret-food-diary-api-openapi.yml
  format: yaml
  label: fatsecret Food Diary API
  slug: fatsecret-food-diary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-food-diary-api-openapi.yml
- filename: fatsecret-foods-api-openapi.yml
  format: yaml
  label: fatsecret Foods API
  slug: fatsecret-foods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-foods-api-openapi.yml
- filename: fatsecret-image-recognition-api-openapi.yml
  format: yaml
  label: fatsecret Image Recognition API
  slug: fatsecret-image-recognition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-image-recognition-api-openapi.yml
- filename: fatsecret-natural-language-processing-api-openapi.yml
  format: yaml
  label: fatsecret Natural Language Processing API
  slug: fatsecret-natural-language-processing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-natural-language-processing-api-openapi.yml
- filename: fatsecret-profile-foods-api-openapi.yml
  format: yaml
  label: fatsecret Profile Foods API
  slug: fatsecret-profile-foods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-profile-foods-api-openapi.yml
- filename: fatsecret-profile-meals-api-openapi.yml
  format: yaml
  label: fatsecret Profile Meals API
  slug: fatsecret-profile-meals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-profile-meals-api-openapi.yml
- filename: fatsecret-recipes-api-openapi.yml
  format: yaml
  label: fatsecret Recipes API
  slug: fatsecret-recipes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-recipes-api-openapi.yml
- filename: fatsecret-reference-api-openapi.yml
  format: yaml
  label: fatsecret Reference API
  slug: fatsecret-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-reference-api-openapi.yml
- filename: fatsecret-weight-tracking-api-openapi.yml
  format: yaml
  label: fatsecret Weight Tracking API
  slug: fatsecret-weight-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-weight-tracking-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fatsecret.com
  spf: true
hosts:
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: platform.fatsecret.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fatsecret Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for fatsecret, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: fatsecret
provider_slug: fatsecret
slug: fatsecret-domain-security
source_filename: fatsecret-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: platform.fatsecret.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: fatsecret.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/security/fatsecret-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Barcode Scanning
- Calories
- Diets
- Image Recognition
- Natural Language Processing
- Exercise
- Fitness
- Food Diary
- Health
- Macronutrients
- Nutrition
- Recipes
- Weight Tracking
---
