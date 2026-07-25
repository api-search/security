---
api_specs:
- filename: microsoft-sql-server-azure-sql-databases-api-openapi.yml
  format: yaml
  label: Microsoft SQL Server Azure SQL Databases API
  slug: microsoft-sql-server-azure-sql-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-sql-server/refs/heads/main/openapi/microsoft-sql-server-azure-sql-databases-api-openapi.yml
- filename: microsoft-sql-server-azure-sql-servers-api-openapi.yml
  format: yaml
  label: Microsoft SQL Server Azure SQL Servers API
  slug: microsoft-sql-server-azure-sql-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-sql-server/refs/heads/main/openapi/microsoft-sql-server-azure-sql-servers-api-openapi.yml
- filename: microsoft-sql-server-data-api-builder-api-openapi.yml
  format: yaml
  label: Microsoft SQL Server Data API Builder API
  slug: microsoft-sql-server-data-api-builder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-sql-server/refs/heads/main/openapi/microsoft-sql-server-data-api-builder-api-openapi.yml
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
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: windows.net
  spf: true
hosts:
- cert_expires: Dec 10 06:59:10 2026 GMT
  host: docs.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: your-server.database.windows.net
  https: false
- cert_expires: Dec 11 02:26:09 2026 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microsoft Sql Server Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft SQL Server, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft SQL Server
provider_slug: microsoft-sql-server
slug: microsoft-sql-server-domain-security
source_filename: microsoft-sql-server-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 06:59:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: your-server.database.windows.net\n  https: false\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: windows.net\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-sql-server/refs/heads/main/security/microsoft-sql-server-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud
- Data Management
- Database
- Enterprise
- Relational Database
- SQL
---
