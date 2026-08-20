---
api_specs:
- filename: matillion-dpc-agents-api-openapi.yml
  format: yaml
  label: Matillion DPC Agents API
  slug: matillion-dpc-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-dpc-agents-api-openapi.yml
- filename: matillion-dpc-environments-api-openapi.yml
  format: yaml
  label: Matillion DPC Environments API
  slug: matillion-dpc-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-dpc-environments-api-openapi.yml
- filename: matillion-dpc-pipeline-executions-api-openapi.yml
  format: yaml
  label: Matillion DPC Pipeline Executions API
  slug: matillion-dpc-pipeline-executions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-dpc-pipeline-executions-api-openapi.yml
- filename: matillion-dpc-projects-api-openapi.yml
  format: yaml
  label: Matillion DPC Projects API
  slug: matillion-dpc-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-dpc-projects-api-openapi.yml
- filename: matillion-dpc-schedules-api-openapi.yml
  format: yaml
  label: Matillion DPC Schedules API
  slug: matillion-dpc-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-dpc-schedules-api-openapi.yml
- filename: matillion-etl-groups-projects-api-openapi.yml
  format: yaml
  label: Matillion ETL Groups & Projects API
  slug: matillion-etl-groups-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-etl-groups-projects-api-openapi.yml
- filename: matillion-etl-jobs-runs-api-openapi.yml
  format: yaml
  label: Matillion ETL Jobs & Runs API
  slug: matillion-etl-jobs-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-etl-jobs-runs-api-openapi.yml
- filename: matillion-etl-schedules-api-openapi.yml
  format: yaml
  label: Matillion ETL Schedules API
  slug: matillion-etl-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-etl-schedules-api-openapi.yml
- filename: matillion-etl-tasks-api-openapi.yml
  format: yaml
  label: Matillion ETL Tasks API
  slug: matillion-etl-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-etl-tasks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: matillion.com
  spf: true
hosts:
- cert_expires: Aug 28 16:05:37 2026 GMT
  host: www.matillion.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 22:17:19 2026 GMT
  host: docs.matillion.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 07:06:19 2026 GMT
  host: eu1.api.matillion.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Matillion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Matillion, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Matillion
provider_slug: matillion
slug: matillion-domain-security
source_filename: matillion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.matillion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 16:05:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.matillion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 22:17:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: eu1.api.matillion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 07:06:19 2026 GMT\n  hsts: null\ndomains:\n- domain: matillion.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/security/matillion-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Integration
- ETL
- ELT
- Data Pipeline
- Cloud Data Warehouse
---
