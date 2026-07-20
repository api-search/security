---
api_specs:
- filename: influxdata-cloud-openapi-original.yml
  format: yaml
  label: InfluxDB Cloud API
  slug: influxdb-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/influxdata/refs/heads/main/openapi/influxdata-cloud-openapi-original.yml
- filename: influxdata-oss-openapi-original.yml
  format: yaml
  label: InfluxDB OSS API
  slug: influxdb-oss-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/influxdata/refs/heads/main/openapi/influxdata-oss-openapi-original.yml
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
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: docs.influxdata.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 10:31:36 2026 GMT
  host: us-east-1-1.aws.cloud2.influxdata.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Influxdata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for InfluxData, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: InfluxData
provider_slug: influxdata
slug: influxdata-domain-security
source_filename: influxdata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.influxdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 06:45:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.influxdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: false\n- host: us-east-1-1.aws.cloud2.influxdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 10:31:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: influxdata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/influxdata/refs/heads/main/security/influxdata-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Time Series Database
- Database
- Monitoring
- Observability
- IoT
- Metrics
- Analytics
- DevOps
- Real-Time Data
- InfluxDB
- Telegraf
- Company
---
