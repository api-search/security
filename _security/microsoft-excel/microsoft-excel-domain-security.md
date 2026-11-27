---
api_specs:
- filename: microsoft-excel-drives-drive-actions-api-openapi.yml
  format: yaml
  label: Microsoft Excel Drives.drive.Actions API
  slug: microsoft-excel-drives-drive-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-excel/openapi/microsoft-excel-drives-drive-actions-api-openapi.yml
- filename: microsoft-excel-drives-drive-functions-api-openapi.yml
  format: yaml
  label: Microsoft Excel Drives.drive.Functions API
  slug: microsoft-excel-drives-drive-functions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-excel/openapi/microsoft-excel-drives-drive-functions-api-openapi.yml
- filename: microsoft-excel-drives-driveitem-api-openapi.yml
  format: yaml
  label: Microsoft Excel Drives.drive Item API
  slug: microsoft-excel-drives-driveitem-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-excel/openapi/microsoft-excel-drives-driveitem-api-openapi.yml
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
  - 0 issue "dtrust.de"
  - 0 issue "entrust.net"
  - 0 issue "globalsign.com"
  - 0 issue "microsoft.com"
  - 0 contactemail "caarecordaware@microsoft.com"
  - 0 iodef "mailto:domains@microsoft.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: office.com
  spf: false
hosts:
- cert_expires: Jan 17 19:55:21 2027 GMT
  host: www.microsoft.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  8 00:23:13 2027 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 12:34:51 2027 GMT
  host: excel.office.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
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
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 19:55:21 2027 GMT\n  hsts: false\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  8 00:23:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: excel.office.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 12:34:51 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: office.com\n  dnssec: true\n  caa:\n  - 0 issue \"dtrust.de\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"microsoft.com\"\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  - 0 iodef \"mailto:domains@microsoft.com\"\n  spf: false\n  dmarc: true\n\
  \  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/microsoft-excel/security/microsoft-excel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Automation
- Data Analysis
- Microsoft
- Microsoft 365
- Office
- Spreadsheets
---
