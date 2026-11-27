---
api_specs:
- filename: microsoft-azure-databricks-accessconnector-api-openapi.yml
  format: yaml
  label: Azure Databricks Access Connector API
  slug: microsoft-azure-databricks-accessconnector-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-databricks/openapi/microsoft-azure-databricks-accessconnector-api-openapi.yml
- filename: microsoft-azure-databricks-delete-api-openapi.yml
  format: yaml
  label: Azure Databricks DELETE API
  slug: microsoft-azure-databricks-delete-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-databricks/openapi/microsoft-azure-databricks-delete-api-openapi.yml
- filename: microsoft-azure-databricks-operations-api-openapi.yml
  format: yaml
  label: Azure Databricks Operations API
  slug: microsoft-azure-databricks-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-databricks/openapi/microsoft-azure-databricks-operations-api-openapi.yml
- filename: microsoft-azure-databricks-privatelinkresources-api-openapi.yml
  format: yaml
  label: Azure Databricks Private Link Resources API
  slug: microsoft-azure-databricks-privatelinkresources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-databricks/openapi/microsoft-azure-databricks-privatelinkresources-api-openapi.yml
- filename: microsoft-azure-databricks-put-api-openapi.yml
  format: yaml
  label: Azure Databricks PUT API
  slug: microsoft-azure-databricks-put-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-databricks/openapi/microsoft-azure-databricks-put-api-openapi.yml
- filename: microsoft-azure-databricks-vnetpeering-api-openapi.yml
  format: yaml
  label: Azure Databricks V Net Peering API
  slug: microsoft-azure-databricks-vnetpeering-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-databricks/openapi/microsoft-azure-databricks-vnetpeering-api-openapi.yml
- filename: microsoft-azure-databricks-workspaces-api-openapi.yml
  format: yaml
  label: Azure Databricks Workspaces API
  slug: microsoft-azure-databricks-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-databricks/openapi/microsoft-azure-databricks-workspaces-api-openapi.yml
- filename: microsoft-azure-databricks-private-endpoint-connections-api-openapi.yml
  format: yaml
  label: Azure Databricks Private Endpoint Connections API
  slug: microsoft-azure-databricks-private-endpoint-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-databricks/openapi/microsoft-azure-databricks-private-endpoint-connections-api-openapi.yml
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
- cert_expires: Jan 17 19:55:21 2027 GMT
  host: www.microsoft.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: <databricks-instance>.azuredatabricks.net
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''<databricks'
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
name: Azure Databricks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Azure Databricks, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Azure Databricks
provider_slug: microsoft-azure-databricks
slug: microsoft-azure-databricks-domain-security
source_filename: microsoft-azure-databricks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 19:55:21 2027 GMT\n  hsts: false\n- host: <databricks-instance>.azuredatabricks.net\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''<databricks'\n  hsts: null\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  8 00:23:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: azuredatabricks.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/microsoft-azure-databricks/security/microsoft-azure-databricks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Apache Spark
- Big Data
- Data Engineering
- Machine Learning
---
