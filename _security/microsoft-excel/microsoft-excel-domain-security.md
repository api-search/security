---
api_specs:
- filename: microsoft-excel-charts-api-openapi.yml
  format: yaml
  label: Microsoft Excel Charts API
  slug: microsoft-excel-charts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-excel/refs/heads/main/openapi/microsoft-excel-charts-api-openapi.yml
- filename: microsoft-excel-functions-api-openapi.yml
  format: yaml
  label: Microsoft Excel Functions API
  slug: microsoft-excel-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-excel/refs/heads/main/openapi/microsoft-excel-functions-api-openapi.yml
- filename: microsoft-excel-named-items-api-openapi.yml
  format: yaml
  label: Microsoft Excel Named Items API
  slug: microsoft-excel-named-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-excel/refs/heads/main/openapi/microsoft-excel-named-items-api-openapi.yml
- filename: microsoft-excel-ranges-api-openapi.yml
  format: yaml
  label: Microsoft Excel Ranges API
  slug: microsoft-excel-ranges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-excel/refs/heads/main/openapi/microsoft-excel-ranges-api-openapi.yml
- filename: microsoft-excel-sessions-api-openapi.yml
  format: yaml
  label: Microsoft Excel Sessions API
  slug: microsoft-excel-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-excel/refs/heads/main/openapi/microsoft-excel-sessions-api-openapi.yml
- filename: microsoft-excel-table-columns-api-openapi.yml
  format: yaml
  label: Microsoft Excel Table Columns API
  slug: microsoft-excel-table-columns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-excel/refs/heads/main/openapi/microsoft-excel-table-columns-api-openapi.yml
- filename: microsoft-excel-table-rows-api-openapi.yml
  format: yaml
  label: Microsoft Excel Table Rows API
  slug: microsoft-excel-table-rows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-excel/refs/heads/main/openapi/microsoft-excel-table-rows-api-openapi.yml
- filename: microsoft-excel-tables-api-openapi.yml
  format: yaml
  label: Microsoft Excel Tables API
  slug: microsoft-excel-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-excel/refs/heads/main/openapi/microsoft-excel-tables-api-openapi.yml
- filename: microsoft-excel-worksheets-api-openapi.yml
  format: yaml
  label: Microsoft Excel Worksheets API
  slug: microsoft-excel-worksheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-excel/refs/heads/main/openapi/microsoft-excel-worksheets-api-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
- caa:
  - 0 iodef "mailto:domains@microsoft.com"
  - 0 issue "digicert.com"
  - 0 issue "dtrust.de"
  - 0 issue "entrust.net"
  - 0 issue "globalsign.com"
  - 0 issue "microsoft.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: office.com
  spf: false
hosts:
- cert_expires: Dec 11 02:26:09 2026 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 03:53:00 2026 GMT
  host: graph.microsoft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 29 23:25:49 2026 GMT
  host: excel.office.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microsoft Excel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Excel, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Excel
provider_slug: microsoft-excel
slug: microsoft-excel-domain-security
source_filename: microsoft-excel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: graph.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 03:53:00 2026 GMT\n  hsts: null\n- host: excel.office.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 23:25:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: office.com\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:domains@microsoft.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"dtrust.de\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"microsoft.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-excel/refs/heads/main/security/microsoft-excel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Automation
- Data Analysis
- Microsoft
- Microsoft-365
- Office
- Spreadsheets
---
