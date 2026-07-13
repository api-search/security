---
api_specs:
- filename: open-meteo-forecast-openapi.yml
  format: yaml
  label: Weather Forecast API
  slug: weather-forecast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-meteo/refs/heads/main/openapi/open-meteo-forecast-openapi.yml
- filename: open-meteo-historical-weather-openapi.yml
  format: yaml
  label: Historical Weather API
  slug: historical-weather-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-meteo/refs/heads/main/openapi/open-meteo-historical-weather-openapi.yml
- filename: open-meteo-ensemble-openapi.yml
  format: yaml
  label: Ensemble API
  slug: ensemble-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-meteo/refs/heads/main/openapi/open-meteo-ensemble-openapi.yml
- filename: open-meteo-climate-openapi.yml
  format: yaml
  label: Climate Change API
  slug: climate-change-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-meteo/refs/heads/main/openapi/open-meteo-climate-openapi.yml
- filename: open-meteo-marine-openapi.yml
  format: yaml
  label: Marine Weather API
  slug: marine-weather-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-meteo/refs/heads/main/openapi/open-meteo-marine-openapi.yml
- filename: open-meteo-air-quality-openapi.yml
  format: yaml
  label: Air Quality API
  slug: air-quality-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-meteo/refs/heads/main/openapi/open-meteo-air-quality-openapi.yml
- filename: open-meteo-flood-openapi.yml
  format: yaml
  label: Flood API
  slug: flood-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-meteo/refs/heads/main/openapi/open-meteo-flood-openapi.yml
- filename: open-meteo-seasonal-openapi.yml
  format: yaml
  label: Seasonal Forecast API
  slug: seasonal-forecast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-meteo/refs/heads/main/openapi/open-meteo-seasonal-openapi.yml
- filename: open-meteo-elevation-openapi.yml
  format: yaml
  label: Elevation API
  slug: elevation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-meteo/refs/heads/main/openapi/open-meteo-elevation-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: open-meteo.com
  spf: true
hosts:
- cert_expires: Aug 12 05:36:20 2026 GMT
  host: open-meteo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 02:36:07 2026 GMT
  host: api.open-meteo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 00:38:44 2026 GMT
  host: archive-api.open-meteo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Meteo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open-Meteo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Open-Meteo
provider_slug: open-meteo
slug: open-meteo-domain-security
source_filename: open-meteo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: open-meteo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 05:36:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.open-meteo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 02:36:07 2026 GMT\n  hsts: null\n- host: archive-api.open-meteo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 00:38:44 2026 GMT\n  hsts: null\ndomains:\n- domain: open-meteo.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-meteo/refs/heads/main/security/open-meteo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Weather
- Forecasts
- Historical Weather
- Air Quality
- Marine
- Climate
- Open Source
- Free
---
