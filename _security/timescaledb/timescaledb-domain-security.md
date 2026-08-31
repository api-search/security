---
api_specs:
- filename: timescaledb-analytics-api-openapi.yml
  format: yaml
  label: TimescaleDB / Tiger Data Analytics API
  slug: timescaledb-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timescaledb/refs/heads/main/openapi/timescaledb-analytics-api-openapi.yml
- filename: timescaledb-auth-api-openapi.yml
  format: yaml
  label: TimescaleDB / Tiger Data Auth API
  slug: timescaledb-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timescaledb/refs/heads/main/openapi/timescaledb-auth-api-openapi.yml
- filename: timescaledb-read-replica-sets-api-openapi.yml
  format: yaml
  label: TimescaleDB / Tiger Data Read Replica Sets API
  slug: timescaledb-read-replica-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timescaledb/refs/heads/main/openapi/timescaledb-read-replica-sets-api-openapi.yml
- filename: timescaledb-services-api-openapi.yml
  format: yaml
  label: TimescaleDB / Tiger Data Services API
  slug: timescaledb-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timescaledb/refs/heads/main/openapi/timescaledb-services-api-openapi.yml
- filename: timescaledb-vpcs-api-openapi.yml
  format: yaml
  label: TimescaleDB / Tiger Data VPCs API
  slug: timescaledb-vpcs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timescaledb/refs/heads/main/openapi/timescaledb-vpcs-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: tigerdata.com
  spf: true
hosts:
- cert_expires: Sep 16 01:48:26 2026 GMT
  host: www.tigerdata.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: console.cloud.tigerdata.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Timescaledb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TimescaleDB / Tiger Data, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: TimescaleDB / Tiger Data
provider_slug: timescaledb
slug: timescaledb-domain-security
source_filename: timescaledb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tigerdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 01:48:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: console.cloud.tigerdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tigerdata.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/timescaledb/refs/heads/main/security/timescaledb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Database
- Time-Series
- PostgreSQL
- Open-Source
- Cloud
- Hypertables
- Continuous Aggregates
- Tiger Cloud
---
