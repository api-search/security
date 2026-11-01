---
api_specs:
- filename: climate-engine-home-api-openapi.yml
  format: yaml
  label: Climate Engine Home API
  slug: climate-engine-home-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/climate-engine/openapi/climate-engine-home-api-openapi.yml
- filename: climate-engine-metadata-api-openapi.yml
  format: yaml
  label: Climate Engine Metadata API
  slug: climate-engine-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/climate-engine/openapi/climate-engine-metadata-api-openapi.yml
- filename: climate-engine-reports-api-openapi.yml
  format: yaml
  label: Climate Engine Reports API
  slug: climate-engine-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/climate-engine/openapi/climate-engine-reports-api-openapi.yml
- filename: climate-engine-raster-export-api-openapi.yml
  format: yaml
  label: Climate Engine Raster/export API
  slug: climate-engine-raster-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/climate-engine/openapi/climate-engine-raster-export-api-openapi.yml
- filename: climate-engine-raster-mapid-api-openapi.yml
  format: yaml
  label: Climate Engine Raster/mapid API
  slug: climate-engine-raster-mapid-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/climate-engine/openapi/climate-engine-raster-mapid-api-openapi.yml
- filename: climate-engine-zonal-stats-api-openapi.yml
  format: yaml
  label: Climate Engine Zonal Stats API
  slug: climate-engine-zonal-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/climate-engine/openapi/climate-engine-zonal-stats-api-openapi.yml
- filename: climate-engine-time-series-api-openapi.yml
  format: yaml
  label: Climate Engine Time Series API
  slug: climate-engine-time-series-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/climate-engine/openapi/climate-engine-time-series-api-openapi.yml
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
hosts_probed: 2
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
source_yaml_url: https://artifacts.apis.io/climate-engine/security/climate-engine-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Climate
- Geospatial
- Remote Sensing
- Satellite
- Earth Observation
---
