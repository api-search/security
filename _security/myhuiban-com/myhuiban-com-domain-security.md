---
api_specs:
- filename: myhuiban-com-auth-api-openapi.yml
  format: yaml
  label: MyHuiban Auth API
  slug: myhuiban-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myhuiban-com/openapi/myhuiban-com-auth-api-openapi.yml
- filename: myhuiban-com-conferences-api-openapi.yml
  format: yaml
  label: MyHuiban Conferences API
  slug: myhuiban-com-conferences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myhuiban-com/openapi/myhuiban-com-conferences-api-openapi.yml
- filename: myhuiban-com-journals-api-openapi.yml
  format: yaml
  label: MyHuiban Journals API
  slug: myhuiban-com-journals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myhuiban-com/openapi/myhuiban-com-journals-api-openapi.yml
- filename: myhuiban-com-researchers-api-openapi.yml
  format: yaml
  label: MyHuiban Researchers API
  slug: myhuiban-com-researchers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myhuiban-com/openapi/myhuiban-com-researchers-api-openapi.yml
- filename: myhuiban-com-statistics-api-openapi.yml
  format: yaml
  label: MyHuiban Statistics API
  slug: myhuiban-com-statistics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myhuiban-com/openapi/myhuiban-com-statistics-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: myhuiban.com
  spf: true
hosts:
- cert_expires: Jan 23 05:32:11 2027 GMT
  host: myhuiban.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MyHuiban Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MyHuiban, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MyHuiban
provider_slug: myhuiban-com
slug: myhuiban-com-domain-security
source_filename: myhuiban-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: myhuiban.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 05:32:11 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: myhuiban.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/myhuiban-com/security/myhuiban-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Conferences
- Indexing
- Academic
- Data
---
