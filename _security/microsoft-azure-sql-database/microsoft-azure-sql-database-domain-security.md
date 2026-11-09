---
api_specs:
- filename: microsoft-azure-sql-database-databases-api-openapi.yml
  format: yaml
  label: Azure SQL Database Databases API
  slug: microsoft-azure-sql-database-databases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-sql-database/openapi/microsoft-azure-sql-database-databases-api-openapi.yml
- filename: microsoft-azure-sql-database-elasticpools-api-openapi.yml
  format: yaml
  label: Azure SQL Database ElasticPools API
  slug: microsoft-azure-sql-database-elasticpools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-sql-database/openapi/microsoft-azure-sql-database-elasticpools-api-openapi.yml
- filename: microsoft-azure-sql-database-failovergroups-api-openapi.yml
  format: yaml
  label: Azure SQL Database FailoverGroups API
  slug: microsoft-azure-sql-database-failovergroups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-sql-database/openapi/microsoft-azure-sql-database-failovergroups-api-openapi.yml
- filename: microsoft-azure-sql-database-servers-api-openapi.yml
  format: yaml
  label: Azure SQL Database Servers API
  slug: microsoft-azure-sql-database-servers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-sql-database/openapi/microsoft-azure-sql-database-servers-api-openapi.yml
- filename: microsoft-azure-sql-database-firewall-rules-api-openapi.yml
  format: yaml
  label: Azure SQL Database Firewall Rules API
  slug: microsoft-azure-sql-database-firewall-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-sql-database/openapi/microsoft-azure-sql-database-firewall-rules-api-openapi.yml
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
  domain: azure.com
  spf: true
hosts:
- cert_expires: Jan 30 14:50:49 2027 GMT
  host: microsoft.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 18:52:15 2027 GMT
  host: portal.azure.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  8 00:23:13 2027 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Microsoft Azure Sql Database Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Azure SQL Database, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Azure SQL Database
provider_slug: microsoft-azure-sql-database
slug: microsoft-azure-sql-database-domain-security
source_filename: microsoft-azure-sql-database-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 14:50:49 2027 GMT\n  hsts: false\n- host: portal.azure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 18:52:15 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  8 00:23:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: azure.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/microsoft-azure-sql-database/security/microsoft-azure-sql-database-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Database
- SQL
- Relational Database
- Microsoft Azure
- Microsoft
- Cloud Database
- Managed Database
- SQL Server
---
