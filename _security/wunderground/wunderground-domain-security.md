---
api_specs:
- filename: wunderground-pws-api.yml
  format: yaml
  label: Weather Underground PWS API
  slug: weather-underground-pws-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wunderground/refs/heads/main/openapi/wunderground-pws-api.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "sectigo.com"
  - 0 issue "digicert.com"
  dmarc: false
  dnssec: false
  domain: wunderground.com
  spf: true
- caa:
  - 10 issue "digicert.com"
  - 0 issue "sectigo.com"
  - 100 issue "letsencrypt.org"
  - 0 issue "globalsign.com"
  - 0 issue "amazon.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: weather.com
  spf: true
hosts:
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: www.wunderground.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: api.weather.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wunderground Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Weather Underground, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Weather Underground
provider_slug: wunderground
slug: wunderground-domain-security
source_filename: wunderground-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wunderground.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: false\n- host: api.weather.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: wunderground.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: false\n- domain: weather.com\n  dnssec: false\n  caa:\n  - 10 issue \"digicert.com\"\n  - 0 issue \"sectigo.com\"\n  - 100 issue \"letsencrypt.org\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wunderground/refs/heads/main/security/wunderground-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Weather
- Personal Weather Stations
- Hyperlocal
- Observations
- Forecasts
- Historical Data
- REST API
---
