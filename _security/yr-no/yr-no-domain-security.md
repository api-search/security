---
api_specs:
- filename: swagger
  format: yaml
  label: Locationforecast API
  slug: locationforecast-api
  spec_type: OpenAPI
  url: https://api.met.no/weatherapi/locationforecast/2.0/swagger
- filename: swagger
  format: yaml
  label: MetAlerts API
  slug: metalerts-api
  spec_type: OpenAPI
  url: https://api.met.no/weatherapi/metalerts/2.0/swagger
- filename: swagger
  format: yaml
  label: Nowcast API
  slug: nowcast-api
  spec_type: OpenAPI
  url: https://api.met.no/weatherapi/nowcast/2.0/swagger
- filename: swagger
  format: yaml
  label: Sunrise API
  slug: sunrise-api
  spec_type: OpenAPI
  url: https://api.met.no/weatherapi/sunrise/3.0/swagger
- filename: swagger
  format: yaml
  label: Oceanforecast API
  slug: oceanforecast-api
  spec_type: OpenAPI
  url: https://api.met.no/weatherapi/oceanforecast/2.0/swagger
- filename: swagger
  format: yaml
  label: Radar API
  slug: radar-api
  spec_type: OpenAPI
  url: https://api.met.no/weatherapi/radar/2.0/swagger
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: yr.no
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: met.no
  spf: true
hosts:
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: www.yr.no
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 06:51:30 2026 GMT
  host: api.met.no
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 24 09:32:46 2027 GMT
  host: frost.met.no
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yr No Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yr, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Yr
provider_slug: yr-no
slug: yr-no-domain-security
source_filename: yr-no-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.yr.no\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: api.met.no\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 06:51:30 2026 GMT\n  hsts: false\n- host: frost.met.no\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 24 09:32:46 2027 GMT\n  hsts: false\ndomains:\n- domain: yr.no\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: met.no\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yr-no/refs/heads/main/security/yr-no-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Weather
- Forecasts
- Meteorology
- Climate
- Norway
- Nordic
- Open Data
- Aviation Weather
- Marine Weather
- Alerts
---
