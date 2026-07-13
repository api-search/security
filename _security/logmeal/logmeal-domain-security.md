---
api_specs:
- filename: logmeal-food-recognition-api-openapi.yml
  format: yaml
  label: LogMeal Food Recognition API
  slug: food-recognition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logmeal/refs/heads/main/openapi/logmeal-food-recognition-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: logmeal.com
  spf: true
hosts:
- cert_expires: Sep 29 13:06:11 2026 GMT
  host: logmeal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 13:12:05 2026 GMT
  host: api.logmeal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Logmeal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LogMeal, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LogMeal
provider_slug: logmeal
slug: logmeal-domain-security
source_filename: logmeal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: logmeal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 13:06:11 2026 GMT\n  hsts: false\n- host: api.logmeal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 13:12:05 2026 GMT\n  hsts: null\ndomains:\n- domain: logmeal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/logmeal/refs/heads/main/security/logmeal-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Computer Vision
- Food
- Image Recognition
- Nutrition
- Semantic Tagging
---
