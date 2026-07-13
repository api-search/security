---
api_specs:
- filename: climate-engine-openapi.yml
  format: yaml
  label: Climate Engine Timeseries API
  slug: climate-engine-timeseries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climate-engine/refs/heads/main/openapi/climate-engine-openapi.yml
- filename: climate-engine-openapi.yml
  format: yaml
  label: Climate Engine Zonal Statistics API
  slug: climate-engine-zonal-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climate-engine/refs/heads/main/openapi/climate-engine-openapi.yml
- filename: climate-engine-openapi.yml
  format: yaml
  label: Climate Engine Raster API
  slug: climate-engine-raster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climate-engine/refs/heads/main/openapi/climate-engine-openapi.yml
- filename: climate-engine-openapi.yml
  format: yaml
  label: Climate Engine Reports API
  slug: climate-engine-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climate-engine/refs/heads/main/openapi/climate-engine-openapi.yml
- filename: climate-engine-openapi.yml
  format: yaml
  label: Climate Engine Dataset Catalog API
  slug: climate-engine-dataset-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climate-engine/refs/heads/main/openapi/climate-engine-openapi.yml
- filename: climate-engine-openapi.yml
  format: yaml
  label: Climate Engine Account API
  slug: climate-engine-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climate-engine/refs/heads/main/openapi/climate-engine-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: climateengine.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: climateengine.org
  spf: true
hosts:
- cert_expires: Aug 18 03:28:01 2026 GMT
  host: www.climateengine.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 05:35:50 2026 GMT
  host: api.climateengine.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Climate Engine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Climate Engine, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Climate Engine
provider_slug: climate-engine
slug: climate-engine-domain-security
source_filename: climate-engine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.climateengine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 03:28:01 2026 GMT\n  hsts: null\n- host: api.climateengine.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 05:35:50 2026 GMT\n  hsts: null\ndomains:\n- domain: climateengine.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: climateengine.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/climate-engine/refs/heads/main/security/climate-engine-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Climate
- Geospatial
- Remote Sensing
- Satellite
- Earth Observation
---
