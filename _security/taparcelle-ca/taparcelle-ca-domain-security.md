---
api_specs:
- filename: taparcelle-ca-decisions-api-openapi.yml
  format: yaml
  label: TaParcelle Decisions API
  slug: taparcelle-ca-decisions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taparcelle-ca/openapi/taparcelle-ca-decisions-api-openapi.yml
- filename: taparcelle-ca-demographics-api-openapi.yml
  format: yaml
  label: TaParcelle Demographics API
  slug: taparcelle-ca-demographics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taparcelle-ca/openapi/taparcelle-ca-demographics-api-openapi.yml
- filename: taparcelle-ca-documents-api-openapi.yml
  format: yaml
  label: TaParcelle Documents API
  slug: taparcelle-ca-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taparcelle-ca/openapi/taparcelle-ca-documents-api-openapi.yml
- filename: taparcelle-ca-parcels-api-openapi.yml
  format: yaml
  label: TaParcelle Parcels API
  slug: taparcelle-ca-parcels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taparcelle-ca/openapi/taparcelle-ca-parcels-api-openapi.yml
- filename: taparcelle-ca-search-api-openapi.yml
  format: yaml
  label: TaParcelle Search API
  slug: taparcelle-ca-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taparcelle-ca/openapi/taparcelle-ca-search-api-openapi.yml
- filename: taparcelle-ca-sectors-api-openapi.yml
  format: yaml
  label: TaParcelle Sectors API
  slug: taparcelle-ca-sectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taparcelle-ca/openapi/taparcelle-ca-sectors-api-openapi.yml
- filename: taparcelle-ca-usage-api-openapi.yml
  format: yaml
  label: TaParcelle Usage API
  slug: taparcelle-ca-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taparcelle-ca/openapi/taparcelle-ca-usage-api-openapi.yml
- filename: taparcelle-ca-zoning-api-openapi.yml
  format: yaml
  label: TaParcelle Zoning API
  slug: taparcelle-ca-zoning-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taparcelle-ca/openapi/taparcelle-ca-zoning-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: taparcelle.ca
  spf: false
hosts:
- cert_expires: Feb  3 00:38:51 2027 GMT
  host: taparcelle.ca
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: TaParcelle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TaParcelle, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: TaParcelle
provider_slug: taparcelle-ca
slug: taparcelle-ca-domain-security
source_filename: taparcelle-ca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: taparcelle.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 00:38:51 2027 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: taparcelle.ca\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/taparcelle-ca/security/taparcelle-ca-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- RealEstate
- DataAggregation
- Quebec
- Property
- API
---
