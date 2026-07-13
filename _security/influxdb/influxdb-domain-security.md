---
api_specs:
- filename: influxdb-openapi.yml
  format: yaml
  label: InfluxDB Cloud API
  slug: influxdb
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/influxdb/refs/heads/main/openapi/influxdb-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: influxdata.com
  spf: true
hosts:
- cert_expires: Sep 23 06:45:30 2026 GMT
  host: www.influxdata.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 19:10:35 2026 GMT
  host: cloud2.influxdata.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Influxdb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for InfluxDB, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: InfluxDB
provider_slug: influxdb
slug: influxdb-domain-security
source_filename: influxdb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.influxdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 06:45:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cloud2.influxdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 19:10:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: influxdata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/influxdb/refs/heads/main/security/influxdb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Database
- Time Series
- Real-Time
- Analytics
---
