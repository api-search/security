---
api_specs:
- filename: waqi-openapi.json
  format: json
  label: WAQI JSON API
  slug: waqi-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/waqi/refs/heads/main/openapi/waqi-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: waqi.info
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aqicn.org
  spf: true
hosts:
- cert_expires: Aug 16 14:10:15 2026 GMT
  host: waqi.info
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug  8 05:59:26 2026 GMT
  host: aqicn.org
  hsts: true
  hsts_max_age: 3600
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 17 14:02:26 2026 GMT
  host: api.waqi.info
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Waqi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for World Air Quality Index (WAQI), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: World Air Quality Index (WAQI)
provider_slug: waqi
slug: waqi-domain-security
source_filename: waqi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: waqi.info\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 16 14:10:15 2026 GMT\n  hsts: false\n- host: aqicn.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug  8 05:59:26 2026 GMT\n  hsts: true\n  hsts_max_age: 3600\n- host: api.waqi.info\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 17 14:02:26 2026 GMT\n  hsts: null\ndomains:\n- domain: waqi.info\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: aqicn.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/waqi/refs/heads/main/security/waqi-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Air Quality
- AQI
- Environment
- Pollution
- Real-Time Data
- Weather
- IoT
- Open Data
---
