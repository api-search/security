---
api_specs:
- filename: azure-databricks-openapi.yml
  format: yaml
  label: Azure Databricks REST API
  slug: azure-databricks-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-databricks/refs/heads/main/openapi/azure-databricks-openapi.yml
- filename: azure-databricks-openapi.yml
  format: yaml
  label: Clusters API
  slug: clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-databricks/refs/heads/main/openapi/azure-databricks-openapi.yml
- filename: azure-databricks-openapi.yml
  format: yaml
  label: Jobs API
  slug: jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-databricks/refs/heads/main/openapi/azure-databricks-openapi.yml
- filename: azure-databricks-openapi.yml
  format: yaml
  label: Workspace API
  slug: workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-databricks/refs/heads/main/openapi/azure-databricks-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: azuredatabricks.net
  spf: true
hosts:
- cert_expires: Dec 11 02:26:09 2026 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: <databricks-instance>.azuredatabricks.net
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''<databricks'
kind: domain-security
layout: security
method: probed
name: Azure Databricks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Azure Databricks, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Azure Databricks
provider_slug: azure-databricks
slug: azure-databricks-domain-security
source_filename: azure-databricks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: <databricks-instance>.azuredatabricks.net\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''<databricks'\n  hsts: null\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: azuredatabricks.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-databricks/refs/heads/main/security/azure-databricks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Apache Spark
- Big Data
- Data Engineering
- Machine Learning
---
