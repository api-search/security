---
api_specs:
- filename: nutritionix-track-openapi.yml
  format: yaml
  label: Nutritionix Track API v2
  slug: nutritionix-track-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutritionix/main/openapi/nutritionix-track-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nutritionix.com
  spf: false
hosts:
- cert_expires: Sep 22 23:59:59 2026 GMT
  host: www.nutritionix.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 23:59:59 2026 GMT
  host: developer.nutritionix.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 23:59:59 2026 GMT
  host: trackapi.nutritionix.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nutritionix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nutritionix, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Nutritionix
provider_slug: nutritionix
slug: nutritionix-domain-security
source_filename: nutritionix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nutritionix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.nutritionix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: trackapi.nutritionix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nutritionix.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nutritionix/refs/heads/main/security/nutritionix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Restaurant
- Health
- Nutrition
- Food
- Fitness
- Public APIs
---
