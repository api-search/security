---
api_specs:
- filename: gender-api-country-of-origin-api-openapi.yml
  format: yaml
  label: Gender API Country Of Origin API
  slug: gender-api-country-of-origin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gender-api/openapi/gender-api-country-of-origin-api-openapi.yml
- filename: gender-api-gender-api-openapi.yml
  format: yaml
  label: Gender API Gender API
  slug: gender-api-gender-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gender-api/openapi/gender-api-gender-api-openapi.yml
- filename: gender-api-statistic-api-openapi.yml
  format: yaml
  label: Gender API Statistic API
  slug: gender-api-statistic-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gender-api/openapi/gender-api-statistic-api-openapi.yml
- filename: gender-api-signup-api-openapi.yml
  format: yaml
  label: Gender API Signup API
  slug: gender-api-signup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gender-api/openapi/gender-api-signup-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gender-api.com
  spf: true
hosts:
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: gender-api.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gender Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gender API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Gender API
provider_slug: gender-api
slug: gender-api-domain-security
source_filename: gender-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gender-api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gender-api.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/gender-api/security/gender-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Demographics
- Gender
- Identity
- Name
- Personal Data
---
