---
api_specs:
- filename: azure-log-analytics-ingestion-api-openapi.yml
  format: yaml
  label: Azure Log Analytics Ingestion API
  slug: azure-log-analytics-ingestion-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-log-analytics/openapi/azure-log-analytics-ingestion-api-openapi.yml
- filename: azure-log-analytics-query-api-openapi.yml
  format: yaml
  label: Azure Log Analytics Query API
  slug: azure-log-analytics-query-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-log-analytics/openapi/azure-log-analytics-query-api-openapi.yml
- filename: azure-log-analytics-saved-searches-api-openapi.yml
  format: yaml
  label: Azure Log Analytics Saved Searches API
  slug: azure-log-analytics-saved-searches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-log-analytics/openapi/azure-log-analytics-saved-searches-api-openapi.yml
- filename: azure-log-analytics-tables-api-openapi.yml
  format: yaml
  label: Azure Log Analytics Tables API
  slug: azure-log-analytics-tables-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-log-analytics/openapi/azure-log-analytics-tables-api-openapi.yml
- filename: azure-log-analytics-workspaces-api-openapi.yml
  format: yaml
  label: Azure Log Analytics Workspaces API
  slug: azure-log-analytics-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-log-analytics/openapi/azure-log-analytics-workspaces-api-openapi.yml
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
- cert_expires: Jan 17 19:55:21 2027 GMT
  host: www.microsoft.com
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
name: Azure Log Analytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Azure Log Analytics, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Azure Log Analytics
provider_slug: azure-log-analytics
slug: azure-log-analytics-domain-security
source_filename: azure-log-analytics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 19:55:21 2027 GMT\n  hsts: false\n- host: portal.azure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 18:52:15 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  8 00:23:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: azure.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/azure-log-analytics/security/azure-log-analytics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Microsoft Azure
- Cloud
- Logging
- Monitoring
---
