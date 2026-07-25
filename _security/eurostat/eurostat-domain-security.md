---
api_specs:
- filename: eurostat-async-api-openapi.yml
  format: yaml
  label: Eurostat Async API
  slug: eurostat-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eurostat/refs/heads/main/openapi/eurostat-async-api-openapi.yml
- filename: eurostat-catalogue-queries-api-openapi.yml
  format: yaml
  label: Eurostat Catalogue queries API
  slug: eurostat-catalogue-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eurostat/refs/heads/main/openapi/eurostat-catalogue-queries-api-openapi.yml
- filename: eurostat-sdmx-2-1-data-queries-api-openapi.yml
  format: yaml
  label: Eurostat SDMX 2.1 Data queries API
  slug: eurostat-sdmx-2-1-data-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eurostat/refs/heads/main/openapi/eurostat-sdmx-2-1-data-queries-api-openapi.yml
- filename: eurostat-sdmx-2-1-navigation-structure-queries-api-openapi.yml
  format: yaml
  label: Eurostat SDMX 2.1 Navigation Structure queries API
  slug: eurostat-sdmx-2-1-navigation-structure-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eurostat/refs/heads/main/openapi/eurostat-sdmx-2-1-navigation-structure-queries-api-openapi.yml
- filename: eurostat-sdmx-2-1-structure-queries-api-openapi.yml
  format: yaml
  label: Eurostat SDMX 2.1 Structure queries API
  slug: eurostat-sdmx-2-1-structure-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eurostat/refs/heads/main/openapi/eurostat-sdmx-2-1-structure-queries-api-openapi.yml
- filename: eurostat-sdmx-3-0-data-queries-api-openapi.yml
  format: yaml
  label: Eurostat SDMX 3.0 Data queries API
  slug: eurostat-sdmx-3-0-data-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eurostat/refs/heads/main/openapi/eurostat-sdmx-3-0-data-queries-api-openapi.yml
- filename: eurostat-sdmx-3-0-structure-queries-api-openapi.yml
  format: yaml
  label: Eurostat SDMX 3.0 Structure queries API
  slug: eurostat-sdmx-3-0-structure-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eurostat/refs/heads/main/openapi/eurostat-sdmx-3-0-structure-queries-api-openapi.yml
- filename: eurostat-statistics-data-queries-api-openapi.yml
  format: yaml
  label: Eurostat Statistics data queries API
  slug: eurostat-statistics-data-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eurostat/refs/heads/main/openapi/eurostat-statistics-data-queries-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: europa.eu
  spf: true
hosts:
- cert_expires: Aug  7 13:10:56 2026 GMT
  host: ec.europa.eu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eurostat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eurostat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Eurostat
provider_slug: eurostat
slug: eurostat-domain-security
source_filename: eurostat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ec.europa.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  7 13:10:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: europa.eu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eurostat/refs/heads/main/security/eurostat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Statistics
- European Union
- Open Data
- Demographics
- Economy
- Trade
- Agriculture
- Transport
- Environment
- SDMX
---
