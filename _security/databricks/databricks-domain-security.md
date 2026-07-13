---
api_specs:
- filename: databricks-openapi.yml
  format: yaml
  label: Databricks
  slug: databricks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databricks/refs/heads/main/openapi/databricks-openapi.yml
- filename: databricks-openapi.yml
  format: yaml
  label: Databricks Clusters API
  slug: clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databricks/refs/heads/main/openapi/databricks-openapi.yml
- filename: databricks-openapi.yml
  format: yaml
  label: Databricks Jobs API
  slug: jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databricks/refs/heads/main/openapi/databricks-openapi.yml
- filename: databricks-openapi.yml
  format: yaml
  label: Databricks Workspace API
  slug: workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databricks/refs/heads/main/openapi/databricks-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "cybertrust.ne.jp"
  - 0 issue "digicert.com"
  - 0 issue "digicert.ne.jp"
  - 0 issue "geotrust.com"
  - 0 issue "intermediatecertificate.digitalcertvalidation.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: databricks.com
  spf: true
hosts:
- cert_expires: Nov 28 23:59:59 2026 GMT
  host: www.databricks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 23:59:59 2026 GMT
  host: docs.databricks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Databricks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Databricks, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Databricks
provider_slug: databricks
slug: databricks-domain-security
source_filename: databricks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.databricks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.databricks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: databricks.com\n  dnssec: true\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"cybertrust.ne.jp\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"digicert.ne.jp\"\n  - 0 issue \"geotrust.com\"\n  - 0 issue \"intermediatecertificate.digitalcertvalidation.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/databricks/refs/heads/main/security/databricks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- Analytics
- Apache Spark
- Big Data
- Clean Rooms
- Cloud Computing
- Data
- Data Analytics
- Data Engineering
- Data Governance
- Delta Lake
- Delta Sharing
- ETL
- Identity Management
- Lakehouse
- Machine Learning
- MLflow
- Model Serving
- Security
- SQL
- Unity Catalog
- Vector Search
- Visualize
---
