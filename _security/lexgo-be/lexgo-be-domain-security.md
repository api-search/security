---
api_specs:
- filename: lexgo-be-events-api-openapi.yml
  format: yaml
  label: lexgo-be Events API
  slug: lexgo-be-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lexgo-be/openapi/lexgo-be-events-api-openapi.yml
- filename: lexgo-be-functions-api-openapi.yml
  format: yaml
  label: lexgo-be Functions API
  slug: lexgo-be-functions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lexgo-be/openapi/lexgo-be-functions-api-openapi.yml
- filename: lexgo-be-jobs-api-openapi.yml
  format: yaml
  label: lexgo-be Jobs API
  slug: lexgo-be-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lexgo-be/openapi/lexgo-be-jobs-api-openapi.yml
- filename: lexgo-be-taxonomies-api-openapi.yml
  format: yaml
  label: lexgo-be Taxonomies API
  slug: lexgo-be-taxonomies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lexgo-be/openapi/lexgo-be-taxonomies-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lexgo.be
  spf: true
hosts:
- cert_expires: Jan 18 21:45:43 2027 GMT
  host: lexgo.be
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: lexgo-be Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for lexgo-be, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: lexgo-be
provider_slug: lexgo-be
slug: lexgo-be-domain-security
source_filename: lexgo-be-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lexgo.be\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 21:45:43 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lexgo.be\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/lexgo-be/security/lexgo-be-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Job Board
- Legal News
- Legal Directory
- Talent Pool
- Trainings
- Legal Tools
---
