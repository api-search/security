---
api_specs:
- filename: memorycarehomes-fyi-academy-api-openapi.yml
  format: yaml
  label: MemoryCareHomes Academy API
  slug: memorycarehomes-fyi-academy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memorycarehomes-fyi/openapi/memorycarehomes-fyi-academy-api-openapi.yml
- filename: memorycarehomes-fyi-admin-api-openapi.yml
  format: yaml
  label: MemoryCareHomes Admin API
  slug: memorycarehomes-fyi-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memorycarehomes-fyi/openapi/memorycarehomes-fyi-admin-api-openapi.yml
- filename: memorycarehomes-fyi-categories-api-openapi.yml
  format: yaml
  label: MemoryCareHomes Categories API
  slug: memorycarehomes-fyi-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memorycarehomes-fyi/openapi/memorycarehomes-fyi-categories-api-openapi.yml
- filename: memorycarehomes-fyi-certificates-api-openapi.yml
  format: yaml
  label: MemoryCareHomes Certificates API
  slug: memorycarehomes-fyi-certificates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memorycarehomes-fyi/openapi/memorycarehomes-fyi-certificates-api-openapi.yml
- filename: memorycarehomes-fyi-listings-api-openapi.yml
  format: yaml
  label: MemoryCareHomes Listings API
  slug: memorycarehomes-fyi-listings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memorycarehomes-fyi/openapi/memorycarehomes-fyi-listings-api-openapi.yml
- filename: memorycarehomes-fyi-places-api-openapi.yml
  format: yaml
  label: MemoryCareHomes Places API
  slug: memorycarehomes-fyi-places-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memorycarehomes-fyi/openapi/memorycarehomes-fyi-places-api-openapi.yml
- filename: memorycarehomes-fyi-product-categories-api-openapi.yml
  format: yaml
  label: MemoryCareHomes Product Categories API
  slug: memorycarehomes-fyi-product-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memorycarehomes-fyi/openapi/memorycarehomes-fyi-product-categories-api-openapi.yml
- filename: memorycarehomes-fyi-products-api-openapi.yml
  format: yaml
  label: MemoryCareHomes Products API
  slug: memorycarehomes-fyi-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memorycarehomes-fyi/openapi/memorycarehomes-fyi-products-api-openapi.yml
- filename: memorycarehomes-fyi-sources-api-openapi.yml
  format: yaml
  label: MemoryCareHomes Sources API
  slug: memorycarehomes-fyi-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memorycarehomes-fyi/openapi/memorycarehomes-fyi-sources-api-openapi.yml
- filename: memorycarehomes-fyi-sponsor-api-openapi.yml
  format: yaml
  label: MemoryCareHomes Sponsor API
  slug: memorycarehomes-fyi-sponsor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memorycarehomes-fyi/openapi/memorycarehomes-fyi-sponsor-api-openapi.yml
- filename: memorycarehomes-fyi-stats-api-openapi.yml
  format: yaml
  label: MemoryCareHomes Stats API
  slug: memorycarehomes-fyi-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memorycarehomes-fyi/openapi/memorycarehomes-fyi-stats-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: memorycarehomes.fyi
  spf: true
hosts:
- cert_expires: Jan 17 22:45:45 2027 GMT
  host: memorycarehomes.fyi
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MemoryCareHomes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MemoryCareHomes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MemoryCareHomes
provider_slug: memorycarehomes-fyi
slug: memorycarehomes-fyi-domain-security
source_filename: memorycarehomes-fyi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: memorycarehomes.fyi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 22:45:45 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: memorycarehomes.fyi\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/memorycarehomes-fyi/security/memorycarehomes-fyi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Senior Care
- Directory
- Licensing
- Data
---
