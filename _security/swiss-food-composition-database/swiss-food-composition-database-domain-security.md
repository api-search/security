---
api_specs:
- filename: swiss-food-composition-database-openapi.json
  format: json
  label: Swiss Food Composition Database API
  slug: swiss-food-composition-database-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swiss-food-composition-database/refs/heads/main/openapi/swiss-food-composition-database-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: naehrwertdaten.ch
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: foodcase-services.com
  spf: true
hosts:
- cert_expires: Nov 24 11:18:49 2026 GMT
  host: naehrwertdaten.ch
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 11:16:57 2026 GMT
  host: api.webapp.prod.blv.foodcase-services.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Swiss Food Composition Database Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Swiss Food Composition Database, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Swiss Food Composition Database
provider_slug: swiss-food-composition-database
slug: swiss-food-composition-database-domain-security
source_filename: swiss-food-composition-database-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: naehrwertdaten.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 11:18:49 2026 GMT\n  hsts: false\n- host: api.webapp.prod.blv.foodcase-services.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 11:16:57 2026 GMT\n  hsts: false\ndomains:\n- domain: naehrwertdaten.ch\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: foodcase-services.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swiss-food-composition-database/refs/heads/main/security/swiss-food-composition-database-domain-security.yml
summary_line: TLSv1.3
tags:
- Food
- Nutrition
- Food Composition
- Health
- Open Data
- Government
- Switzerland
- Reference Data
- Public Sector
- Research
---
