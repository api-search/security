---
api_specs:
- filename: noaa-alerts-api-openapi.yml
  format: yaml
  label: NOAA Alerts API
  slug: noaa-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa/refs/heads/main/openapi/noaa-alerts-api-openapi.yml
- filename: noaa-aviation-api-openapi.yml
  format: yaml
  label: NOAA Aviation API
  slug: noaa-aviation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa/refs/heads/main/openapi/noaa-aviation-api-openapi.yml
- filename: noaa-glossary-api-openapi.yml
  format: yaml
  label: NOAA Glossary API
  slug: noaa-glossary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa/refs/heads/main/openapi/noaa-glossary-api-openapi.yml
- filename: noaa-gridpoints-api-openapi.yml
  format: yaml
  label: NOAA Gridpoints API
  slug: noaa-gridpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa/refs/heads/main/openapi/noaa-gridpoints-api-openapi.yml
- filename: noaa-icons-api-openapi.yml
  format: yaml
  label: NOAA Icons API
  slug: noaa-icons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa/refs/heads/main/openapi/noaa-icons-api-openapi.yml
- filename: noaa-navigational-data-api-openapi.yml
  format: yaml
  label: NOAA Navigational Data API
  slug: noaa-navigational-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa/refs/heads/main/openapi/noaa-navigational-data-api-openapi.yml
- filename: noaa-offices-api-openapi.yml
  format: yaml
  label: NOAA Offices API
  slug: noaa-offices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa/refs/heads/main/openapi/noaa-offices-api-openapi.yml
- filename: noaa-points-api-openapi.yml
  format: yaml
  label: NOAA Points API
  slug: noaa-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa/refs/heads/main/openapi/noaa-points-api-openapi.yml
- filename: noaa-products-api-openapi.yml
  format: yaml
  label: NOAA Products API
  slug: noaa-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa/refs/heads/main/openapi/noaa-products-api-openapi.yml
- filename: noaa-radar-api-openapi.yml
  format: yaml
  label: NOAA Radar API
  slug: noaa-radar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa/refs/heads/main/openapi/noaa-radar-api-openapi.yml
- filename: noaa-radio-api-openapi.yml
  format: yaml
  label: NOAA Radio API
  slug: noaa-radio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa/refs/heads/main/openapi/noaa-radio-api-openapi.yml
- filename: noaa-stations-api-openapi.yml
  format: yaml
  label: NOAA Stations API
  slug: noaa-stations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa/refs/heads/main/openapi/noaa-stations-api-openapi.yml
- filename: noaa-thumbnails-api-openapi.yml
  format: yaml
  label: NOAA Thumbnails API
  slug: noaa-thumbnails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa/refs/heads/main/openapi/noaa-thumbnails-api-openapi.yml
- filename: noaa-weather-data-api-openapi.yml
  format: yaml
  label: NOAA Weather Data API
  slug: noaa-weather-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa/refs/heads/main/openapi/noaa-weather-data-api-openapi.yml
- filename: noaa-zones-api-openapi.yml
  format: yaml
  label: NOAA Zones API
  slug: noaa-zones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa/refs/heads/main/openapi/noaa-zones-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "sectigo.com"
  - 0 issue "entrust.net"
  - 0 issue "amazon.com"
  - 0 issue "godaddy.com"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: noaa.gov
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: weather.gov
  spf: false
hosts:
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: www.noaa.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 17:22:04 2026 GMT
  host: www.weather.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 17:22:04 2026 GMT
  host: api.weather.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Noaa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NOAA, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: NOAA
provider_slug: noaa
slug: noaa-domain-security
source_filename: noaa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.noaa.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: null\n- host: www.weather.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 17:22:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.weather.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 17:22:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: noaa.gov\n  dnssec: true\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: weather.gov\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/noaa/refs/heads/main/security/noaa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Weather
- Climate
- Forecast
- Alerts
- Ocean
- Tides
- Aviation Weather
- Government
- Open Data
- Environmental
---
