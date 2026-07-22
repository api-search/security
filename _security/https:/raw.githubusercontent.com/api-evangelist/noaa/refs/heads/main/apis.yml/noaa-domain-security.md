---
api_specs:
- filename: openapi.json
  format: json
  label: National Weather Service API
  slug: national-weather-service-api
  spec_type: OpenAPI
  url: https://api.weather.gov/openapi.json
- filename: openapi.yaml
  format: yaml
  label: Aviation Weather API
  slug: aviation-weather-api
  spec_type: OpenAPI
  url: https://aviationweather.gov/data/schema/openapi.yaml
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
provider_slug: https://raw.githubusercontent.com/api-evangelist/noaa/refs/heads/main/apis.yml
slug: noaa-domain-security
source_filename: noaa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.noaa.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: null\n- host: www.weather.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 17:22:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.weather.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 17:22:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: noaa.gov\n  dnssec: true\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: weather.gov\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/https://raw.githubusercontent.com/api-evangelist/noaa/refs/heads/main/apis.yml/refs/heads/main/security/noaa-domain-security.yml
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
