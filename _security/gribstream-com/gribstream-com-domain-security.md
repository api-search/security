---
api_specs:
- filename: gribstream-com-account-api-openapi.yml
  format: yaml
  label: gribstream-com Account API
  slug: gribstream-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gribstream-com/openapi/gribstream-com-account-api-openapi.yml
- filename: gribstream-com-catalog-api-openapi.yml
  format: yaml
  label: gribstream-com Catalog API
  slug: gribstream-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gribstream-com/openapi/gribstream-com-catalog-api-openapi.yml
- filename: gribstream-com-grid-coordinates-api-openapi.yml
  format: yaml
  label: gribstream-com Grid coordinates API
  slug: gribstream-com-grid-coordinates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gribstream-com/openapi/gribstream-com-grid-coordinates-api-openapi.yml
- filename: gribstream-com-weather-data-api-openapi.yml
  format: yaml
  label: gribstream-com Weather data API
  slug: gribstream-com-weather-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gribstream-com/openapi/gribstream-com-weather-data-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gribstream.com
  spf: true
hosts:
- host: gribstream.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gribstream Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for gribstream-com, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: gribstream-com
provider_slug: gribstream-com
slug: gribstream-com-domain-security
source_filename: gribstream-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gribstream.com\n  https: false\ndomains:\n- domain: gribstream.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/gribstream-com/security/gribstream-com-domain-security.yml
summary_line: DMARC
tags:
- Company
- Weather
- API
- Forecast
- Data
---
