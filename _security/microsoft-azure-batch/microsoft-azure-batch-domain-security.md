---
api_specs:
- filename: microsoft-azure-batch-batch-service-openapi.json
  format: json
  label: Azure Batch Service API
  slug: microsoft-azure-batch-batch-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-batch/refs/heads/main/openapi/_original/microsoft-azure-batch-batch-service-openapi.json
- filename: microsoft-azure-batch-management-openapi.json
  format: json
  label: Azure Batch Management API
  slug: microsoft-azure-batch-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-batch/refs/heads/main/openapi/_original/microsoft-azure-batch-management-openapi.json
- filename: microsoft-azure-batch-jobs-api-openapi.yml
  format: yaml
  label: microsoft-azure-batch Jobs API
  slug: microsoft-azure-batch-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-batch/refs/heads/main/openapi/microsoft-azure-batch-jobs-api-openapi.yml
- filename: microsoft-azure-batch-pools-api-openapi.yml
  format: yaml
  label: microsoft-azure-batch Pools API
  slug: microsoft-azure-batch-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-batch/refs/heads/main/openapi/microsoft-azure-batch-pools-api-openapi.yml
- filename: microsoft-azure-batch-tasks-api-openapi.yml
  format: yaml
  label: microsoft-azure-batch Tasks API
  slug: microsoft-azure-batch-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-batch/refs/heads/main/openapi/microsoft-azure-batch-tasks-api-openapi.yml
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
  dmarc_policy: none
  dnssec: false
  domain: azure.com
  spf: true
hosts:
- cert_expires: Jan 17 19:55:21 2027 GMT
  host: www.microsoft.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 25 12:39:07 2027 GMT
  host: portal.azure.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 02:26:09 2026 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Microsoft Azure Batch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Azure Batch, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Azure Batch
provider_slug: microsoft-azure-batch
slug: microsoft-azure-batch-domain-security
source_filename: microsoft-azure-batch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 19:55:21 2027 GMT\n  hsts: false\n- host: portal.azure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 12:39:07 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: azure.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-batch/refs/heads/main/security/microsoft-azure-batch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Batch
- Compute
- Job Scheduling
- High Performance Computing
- Cloud
- Microsoft
- Azure
- Parallel Processing
- Scheduling
- Infrastructure
---
