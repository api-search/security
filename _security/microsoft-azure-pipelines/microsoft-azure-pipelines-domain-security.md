---
api_specs:
- filename: api
  format: yaml
  label: Azure Pipelines REST API
  slug: azure-pipelines-rest-api
  spec_type: OpenAPI
  url: https://dev.azure.com/{organization}/_apis/public/api
- filename: azure-pipelines-build-api-openapi.yml
  format: yaml
  label: Azure Pipelines Build REST API
  slug: azure-pipelines-build-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-pipelines/refs/heads/main/openapi/azure-pipelines-build-api-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: azure.com
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Sep 21 18:15:50 2026 GMT
  host: dev.azure.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 22:04:48 2026 GMT
  host: azure.microsoft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 02:26:09 2026 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microsoft Azure Pipelines Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Azure Pipelines, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Azure Pipelines
provider_slug: microsoft-azure-pipelines
slug: microsoft-azure-pipelines-domain-security
source_filename: microsoft-azure-pipelines-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dev.azure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 18:15:50 2026 GMT\n  hsts: null\n- host: azure.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 22:04:48 2026 GMT\n  hsts: null\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: azure.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-pipelines/refs/heads/main/security/microsoft-azure-pipelines-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automation
- Build
- CI/CD
- Deployment
- DevOps
- Pipelines
---
