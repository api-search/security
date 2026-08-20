---
api_specs:
- filename: national-weather-service-alerts-api-openapi.yml
  format: yaml
  label: National Weather Service Alerts API
  slug: national-weather-service-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-weather-service/refs/heads/main/openapi/national-weather-service-alerts-api-openapi.yml
- filename: national-weather-service-aviation-api-openapi.yml
  format: yaml
  label: National Weather Service Aviation API
  slug: national-weather-service-aviation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-weather-service/refs/heads/main/openapi/national-weather-service-aviation-api-openapi.yml
- filename: national-weather-service-glossary-api-openapi.yml
  format: yaml
  label: National Weather Service Glossary API
  slug: national-weather-service-glossary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-weather-service/refs/heads/main/openapi/national-weather-service-glossary-api-openapi.yml
- filename: national-weather-service-gridpoints-api-openapi.yml
  format: yaml
  label: National Weather Service Gridpoints API
  slug: national-weather-service-gridpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-weather-service/refs/heads/main/openapi/national-weather-service-gridpoints-api-openapi.yml
- filename: national-weather-service-icons-api-openapi.yml
  format: yaml
  label: National Weather Service Icons API
  slug: national-weather-service-icons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-weather-service/refs/heads/main/openapi/national-weather-service-icons-api-openapi.yml
- filename: national-weather-service-offices-api-openapi.yml
  format: yaml
  label: National Weather Service Offices API
  slug: national-weather-service-offices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-weather-service/refs/heads/main/openapi/national-weather-service-offices-api-openapi.yml
- filename: national-weather-service-points-api-openapi.yml
  format: yaml
  label: National Weather Service Points API
  slug: national-weather-service-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-weather-service/refs/heads/main/openapi/national-weather-service-points-api-openapi.yml
- filename: national-weather-service-products-api-openapi.yml
  format: yaml
  label: National Weather Service Products API
  slug: national-weather-service-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-weather-service/refs/heads/main/openapi/national-weather-service-products-api-openapi.yml
- filename: national-weather-service-radar-api-openapi.yml
  format: yaml
  label: National Weather Service Radar API
  slug: national-weather-service-radar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-weather-service/refs/heads/main/openapi/national-weather-service-radar-api-openapi.yml
- filename: national-weather-service-radio-api-openapi.yml
  format: yaml
  label: National Weather Service Radio API
  slug: national-weather-service-radio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-weather-service/refs/heads/main/openapi/national-weather-service-radio-api-openapi.yml
- filename: national-weather-service-stations-api-openapi.yml
  format: yaml
  label: National Weather Service Stations API
  slug: national-weather-service-stations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-weather-service/refs/heads/main/openapi/national-weather-service-stations-api-openapi.yml
- filename: national-weather-service-thumbnails-api-openapi.yml
  format: yaml
  label: National Weather Service Thumbnails API
  slug: national-weather-service-thumbnails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-weather-service/refs/heads/main/openapi/national-weather-service-thumbnails-api-openapi.yml
- filename: national-weather-service-zones-api-openapi.yml
  format: yaml
  label: National Weather Service Zones API
  slug: national-weather-service-zones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-weather-service/refs/heads/main/openapi/national-weather-service-zones-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: weather.gov
  spf: false
hosts:
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
name: National Weather Service Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Weather Service, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=reject).'
provider_name: National Weather Service
provider_slug: national-weather-service
slug: national-weather-service-domain-security
source_filename: national-weather-service-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.weather.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 17:22:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.weather.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 17:22:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: weather.gov\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-weather-service/refs/heads/main/security/national-weather-service-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal-Government
- Forecasting
- Weather
---
