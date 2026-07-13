---
api_specs:
- filename: colorfulclouds-caiyun-weather-openapi.yml
  format: yaml
  label: Caiyun Weather API
  slug: caiyun-weather-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colorfulclouds/refs/heads/main/openapi/colorfulclouds-caiyun-weather-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: caiyunapp.com
  spf: true
hosts:
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: caiyunapp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: docs.caiyunapp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: api.caiyunapp.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Colorfulclouds Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ColorfulClouds, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ColorfulClouds
provider_slug: colorfulclouds
slug: colorfulclouds-domain-security
source_filename: colorfulclouds-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: caiyunapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: false\n- host: docs.caiyunapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: false\n- host: api.caiyunapp.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: caiyunapp.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/colorfulclouds/refs/heads/main/security/colorfulclouds-domain-security.yml
summary_line: TLSv1.3
tags:
- Weather
- Forecasting
- Air Quality
- Precipitation
- Hyperlocal
- Geospatial
- China
---
