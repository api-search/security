---
api_specs:
- filename: wis2-gdc.weather.gc.ca
  format: yaml
  label: WIS2 Global Discovery Catalogue API
  slug: wis2-global-discovery-catalogue-api
  spec_type: OpenAPI
  url: https://wis2-gdc.weather.gc.ca
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wmo.int
  spf: true
hosts:
- cert_expires: Aug 17 11:31:41 2026 GMT
  host: wmo.int
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  7 11:28:02 2026 GMT
  host: worldweather.wmo.int
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 23:59:59 2026 GMT
  host: oscar.wmo.int
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wmo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for World Meteorological Organization, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: World Meteorological Organization
provider_slug: wmo
slug: wmo-domain-security
source_filename: wmo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wmo.int\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 11:31:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: worldweather.wmo.int\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 11:28:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: oscar.wmo.int\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: wmo.int\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wmo/refs/heads/main/security/wmo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Weather
- Climate
- Hydrology
- Meteorology
- International Organization
- United Nations
- Open Data
---
