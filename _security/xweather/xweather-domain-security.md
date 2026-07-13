---
api_specs:
- filename: xweather-weather-api-openapi.yml
  format: yaml
  label: Xweather Weather API
  slug: xweather
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xweather/refs/heads/main/openapi/xweather-weather-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: xweather.com
  spf: true
hosts:
- cert_expires: Sep 21 07:19:01 2026 GMT
  host: xweather.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 07:39:58 2026 GMT
  host: www.xweather.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: data.api.xweather.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Xweather Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xweather, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Xweather
provider_slug: xweather
slug: xweather-domain-security
source_filename: xweather-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xweather.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 07:19:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.xweather.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 07:39:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: data.api.xweather.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: xweather.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xweather/refs/heads/main/security/xweather-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Air Quality
- Company
- Data
- Forecasts
- Lightning
- Maritime
- Observations
- Severe Weather
- Weather
---
