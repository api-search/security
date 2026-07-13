---
api_specs:
- filename: air-quality-programmatic-apis-openapi.yml
  format: yaml
  label: AQICN Real-Time Air Quality API
  slug: air-quality-programmatic-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/air-quality-programmatic-apis/refs/heads/main/openapi/air-quality-programmatic-apis-openapi.yml
- filename: aqicn-json-api-openapi.yaml
  format: yaml
  label: AQICN JSON Air Quality API
  slug: aqicn-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/air-quality-programmatic-apis/refs/heads/main/openapi/aqicn-json-api-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aqicn.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: waqi.info
  spf: true
hosts:
- cert_expires: Aug  8 05:59:26 2026 GMT
  host: aqicn.org
  hsts: true
  hsts_max_age: 3600
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 17 23:04:00 2026 GMT
  host: tiles.aqicn.org
  hsts: true
  hsts_max_age: 15768000
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
name: Air Quality Programmatic Apis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Air Quality Programmatic APIs, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Air Quality Programmatic APIs
provider_slug: air-quality-programmatic-apis
slug: air-quality-programmatic-apis-domain-security
source_filename: air-quality-programmatic-apis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aqicn.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug  8 05:59:26 2026 GMT\n  hsts: true\n  hsts_max_age: 3600\n- host: tiles.aqicn.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 17 23:04:00 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: api.waqi.info\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 17 14:02:26 2026 GMT\n  hsts: null\ndomains:\n- domain: aqicn.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: waqi.info\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/air-quality-programmatic-apis/refs/heads/main/security/air-quality-programmatic-apis-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Air Quality
- Environment
- EPA
- Open Data
- Public Health
- IoT
- Government Data
- Real-Time Data
---
