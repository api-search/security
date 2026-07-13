---
api_specs:
- filename: matillion-openapi.yml
  format: yaml
  label: DPC Projects
  slug: dpc-projects
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-openapi.yml
- filename: matillion-openapi.yml
  format: yaml
  label: DPC Environments
  slug: dpc-environments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-openapi.yml
- filename: matillion-openapi.yml
  format: yaml
  label: DPC Pipeline Executions
  slug: dpc-pipeline-executions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-openapi.yml
- filename: matillion-openapi.yml
  format: yaml
  label: DPC Schedules
  slug: dpc-schedules
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-openapi.yml
- filename: matillion-openapi.yml
  format: yaml
  label: DPC Agents
  slug: dpc-agents
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-openapi.yml
- filename: matillion-openapi.yml
  format: yaml
  label: ETL Groups & Projects (legacy)
  slug: etl-groups-projects
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-openapi.yml
- filename: matillion-openapi.yml
  format: yaml
  label: ETL Jobs & Runs (legacy)
  slug: etl-jobs-runs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-openapi.yml
- filename: matillion-openapi.yml
  format: yaml
  label: ETL Tasks (legacy)
  slug: etl-tasks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-openapi.yml
- filename: matillion-openapi.yml
  format: yaml
  label: ETL Schedules (legacy)
  slug: etl-schedules
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-openapi.yml
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
- Data Pipelines
- Cloud Data Warehouse
---
