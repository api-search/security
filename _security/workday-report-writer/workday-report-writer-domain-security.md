---
api_specs:
- filename: workday-report-writer-agentdefinition-api-openapi.yml
  format: yaml
  label: Workday Report Writer agentDefinition API
  slug: workday-report-writer-agentdefinition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-report-writer/refs/heads/main/openapi/workday-report-writer-agentdefinition-api-openapi.yml
- filename: workday-report-writer-buckets-api-openapi.yml
  format: yaml
  label: Workday Report Writer Buckets API
  slug: workday-report-writer-buckets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-report-writer/refs/heads/main/openapi/workday-report-writer-buckets-api-openapi.yml
- filename: workday-report-writer-custom-reports-api-openapi.yml
  format: yaml
  label: Workday Report Writer Custom Reports API
  slug: workday-report-writer-custom-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-report-writer/refs/heads/main/openapi/workday-report-writer-custom-reports-api-openapi.yml
- filename: workday-report-writer-data-change-tasks-api-openapi.yml
  format: yaml
  label: Workday Report Writer Data Change Tasks API
  slug: workday-report-writer-data-change-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-report-writer/refs/heads/main/openapi/workday-report-writer-data-change-tasks-api-openapi.yml
- filename: workday-report-writer-data-sources-api-openapi.yml
  format: yaml
  label: Workday Report Writer Data Sources API
  slug: workday-report-writer-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-report-writer/refs/heads/main/openapi/workday-report-writer-data-sources-api-openapi.yml
- filename: workday-report-writer-datasets-api-openapi.yml
  format: yaml
  label: Workday Report Writer Datasets API
  slug: workday-report-writer-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-report-writer/refs/heads/main/openapi/workday-report-writer-datasets-api-openapi.yml
- filename: workday-report-writer-query-execution-api-openapi.yml
  format: yaml
  label: Workday Report Writer Query Execution API
  slug: workday-report-writer-query-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-report-writer/refs/heads/main/openapi/workday-report-writer-query-execution-api-openapi.yml
- filename: workday-report-writer-tables-api-openapi.yml
  format: yaml
  label: Workday Report Writer Tables API
  slug: workday-report-writer-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-report-writer/refs/heads/main/openapi/workday-report-writer-tables-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: workday.com
  spf: true
hosts:
- cert_expires: Aug 21 03:09:01 2026 GMT
  host: developer.workday.com
  hsts: true
  hsts_max_age: 15638400
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: www.workday.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 03:30:49 2026 GMT
  host: wd2-impl-services1.workday.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Workday Report Writer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Workday Report Writer, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Workday Report Writer
provider_slug: workday-report-writer
slug: workday-report-writer-domain-security
source_filename: workday-report-writer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.workday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 03:09:01 2026 GMT\n  hsts: true\n  hsts_max_age: 15638400\n- host: www.workday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: wd2-impl-services1.workday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 03:30:49 2026 GMT\n  hsts: null\ndomains:\n- domain: workday.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-report-writer/refs/heads/main/security/workday-report-writer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Enterprise
- ERP
- Financials
- HRMS
- Reporting
- Software-as-a-Service
---
