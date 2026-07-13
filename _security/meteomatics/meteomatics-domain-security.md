---
api_specs:
- filename: meteomatics-weather-openapi.yml
  format: yaml
  label: Meteomatics Weather API
  slug: meteomatics-weather-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meteomatics/refs/heads/main/openapi/meteomatics-weather-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: meteomatics.com
  spf: true
hosts:
- cert_expires: Sep 14 09:01:29 2026 GMT
  host: www.meteomatics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 21 23:59:59 2026 GMT
  host: api.meteomatics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Meteomatics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Meteomatics, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Meteomatics
provider_slug: meteomatics
slug: meteomatics-domain-security
source_filename: meteomatics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.meteomatics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 09:01:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.meteomatics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: meteomatics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meteomatics/refs/heads/main/security/meteomatics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Weather
- Forecast
- Climate
- Historical Weather
- Marine
- Environmental Data
- Hyperlocal
- Meteorology
- Time Series
- Geospatial
---
