---
api_specs:
- filename: nutrical-solution-ltd-openapi.yml
  format: yaml
  label: NutriCal Food & Nutrition API
  slug: nutrical-food-nutrition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutrical-solution-ltd/refs/heads/main/openapi/nutrical-solution-ltd-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nutrical.co
  spf: true
hosts:
- cert_expires: Sep  7 18:37:34 2026 GMT
  host: nutrical.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: api.nutrical.co
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: preprodapi.nutrical.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nutrical Solution Ltd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nutrical Solution Ltd, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nutrical Solution Ltd
provider_slug: nutrical-solution-ltd
slug: nutrical-solution-ltd-domain-security
source_filename: nutrical-solution-ltd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nutrical.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 18:37:34 2026 GMT\n  hsts: false\n- host: api.nutrical.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: null\n- host: preprodapi.nutrical.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: nutrical.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nutrical-solution-ltd/refs/heads/main/security/nutrical-solution-ltd-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Food
- Nutrition
- Health
- Recipes
- Meal Plans
- Food Labeling
- Compliance
- Restaurants
- GCC
---
