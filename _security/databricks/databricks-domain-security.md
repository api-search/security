---
api_specs:
- filename: databricks-clusters-api-openapi.yml
  format: yaml
  label: Databricks Clusters API
  slug: databricks-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databricks/refs/heads/main/openapi/databricks-clusters-api-openapi.yml
- filename: databricks-jobs-api-openapi.yml
  format: yaml
  label: Databricks Jobs API
  slug: databricks-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databricks/refs/heads/main/openapi/databricks-jobs-api-openapi.yml
- filename: databricks-workspace-api-openapi.yml
  format: yaml
  label: Databricks Workspace API
  slug: databricks-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databricks/refs/heads/main/openapi/databricks-workspace-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "www.digicert.com"
  - 0 issuewild "1and1.digitalcertvalidation.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: databricks.com
  spf: true
hosts:
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: www.databricks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: docs.databricks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
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
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.databricks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.databricks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: databricks.com\n  dnssec: true\n  caa:\n  - 0 issue \"www.digicert.com\"\n  - 0 issuewild \"1and1.digitalcertvalidation.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/databricks/refs/heads/main/security/databricks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cleanroom
- Databricks
- Artificial Intelligence
- Analytics
- Apache Spark
- Big Data
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
- Data Catalog
---
