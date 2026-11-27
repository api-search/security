---
api_specs:
- filename: lexbase-pt-diploma-api-openapi.yml
  format: yaml
  label: Lexbase Diploma API
  slug: lexbase-pt-diploma-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lexbase-pt/openapi/lexbase-pt-diploma-api-openapi.yml
- filename: lexbase-pt-diplomas-api-openapi.yml
  format: yaml
  label: Lexbase Diplomas API
  slug: lexbase-pt-diplomas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lexbase-pt/openapi/lexbase-pt-diplomas-api-openapi.yml
- filename: lexbase-pt-fragment-api-openapi.yml
  format: yaml
  label: Lexbase Fragment API
  slug: lexbase-pt-fragment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lexbase-pt/openapi/lexbase-pt-fragment-api-openapi.yml
- filename: lexbase-pt-health-api-openapi.yml
  format: yaml
  label: Lexbase Health API
  slug: lexbase-pt-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lexbase-pt/openapi/lexbase-pt-health-api-openapi.yml
- filename: lexbase-pt-search-api-openapi.yml
  format: yaml
  label: Lexbase Search API
  slug: lexbase-pt-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lexbase-pt/openapi/lexbase-pt-search-api-openapi.yml
- filename: lexbase-pt-themes-api-openapi.yml
  format: yaml
  label: Lexbase Themes API
  slug: lexbase-pt-themes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lexbase-pt/openapi/lexbase-pt-themes-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lexbase.pt
  spf: true
hosts:
- cert_expires: Feb  7 15:07:35 2027 GMT
  host: lexbase.pt
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lexbase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lexbase, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lexbase
provider_slug: lexbase-pt
slug: lexbase-pt-domain-security
source_filename: lexbase-pt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lexbase.pt\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 15:07:35 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lexbase.pt\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/lexbase-pt/security/lexbase-pt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Legal Tech
- PortugueseLaw
- Search
- AI Integration
---
