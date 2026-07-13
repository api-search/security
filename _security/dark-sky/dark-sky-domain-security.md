---
api_specs:
- filename: openapi.yml
  format: yaml
  label: Dark Sky Forecast API
  slug: dark-sky-forecast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dark-sky/refs/heads/main/openapi/openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: darksky.net
  spf: true
hosts:
- cert_expires: Aug 10 06:01:04 2026 GMT
  host: darksky.net
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.darksky.net
  https: false
kind: domain-security
layout: security
method: probed
name: Dark Sky Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dark Sky, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Dark Sky
provider_slug: dark-sky
slug: dark-sky-domain-security
source_filename: dark-sky-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: darksky.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 06:01:04 2026 GMT\n  hsts: null\n- host: api.darksky.net\n  https: false\ndomains:\n- domain: darksky.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dark-sky/refs/heads/main/security/dark-sky-domain-security.yml
summary_line: TLSv1.3
tags:
- Weather
- Forecast
- Hyperlocal
- Precipitation
- Machine Learning
- REST
- Apple
---
