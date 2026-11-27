---
api_specs:
- filename: geogridapi-io-account-api-openapi.yml
  format: yaml
  label: GeoGridAPI Account API
  slug: geogridapi-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geogridapi-io/openapi/geogridapi-io-account-api-openapi.yml
- filename: geogridapi-io-batches-api-openapi.yml
  format: yaml
  label: GeoGridAPI Batches API
  slug: geogridapi-io-batches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geogridapi-io/openapi/geogridapi-io-batches-api-openapi.yml
- filename: geogridapi-io-grids-api-openapi.yml
  format: yaml
  label: GeoGridAPI Grids API
  slug: geogridapi-io-grids-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geogridapi-io/openapi/geogridapi-io-grids-api-openapi.yml
- filename: geogridapi-io-listings-api-openapi.yml
  format: yaml
  label: GeoGridAPI Listings API
  slug: geogridapi-io-listings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geogridapi-io/openapi/geogridapi-io-listings-api-openapi.yml
- filename: geogridapi-io-schedules-api-openapi.yml
  format: yaml
  label: GeoGridAPI Schedules API
  slug: geogridapi-io-schedules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geogridapi-io/openapi/geogridapi-io-schedules-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: geogridapi.io
  spf: true
hosts:
- cert_expires: Jan 14 11:13:21 2027 GMT
  host: geogridapi.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GeoGridAPI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GeoGridAPI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GeoGridAPI
provider_slug: geogridapi-io
slug: geogridapi-io-domain-security
source_filename: geogridapi-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: geogridapi.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 11:13:21 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: geogridapi.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/geogridapi-io/security/geogridapi-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- GeoGridAPI
- Mapping
- SEO
- Business
---
