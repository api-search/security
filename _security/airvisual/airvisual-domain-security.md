---
api_specs:
- filename: openapi.json
  format: json
  label: IQAir AirVisual API
  slug: iqair-airvisual-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airvisual/refs/heads/main/openapi/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: iqair.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: airvisual.com
  spf: true
hosts:
- cert_expires: Sep 23 21:03:49 2026 GMT
  host: www.iqair.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  2 23:59:59 2027 GMT
  host: api.airvisual.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Airvisual Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IQAir AirVisual, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: IQAir AirVisual
provider_slug: airvisual
slug: airvisual-domain-security
source_filename: airvisual-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.iqair.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 21:03:49 2026 GMT\n  hsts: null\n- host: api.airvisual.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  2 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: iqair.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: airvisual.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airvisual/refs/heads/main/security/airvisual-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Air Quality
- AQI
- PM2.5
- Weather
- Pollution
- Environmental Data
- Real-Time Data
---
