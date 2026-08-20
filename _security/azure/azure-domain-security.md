---
api_specs:
- filename: azure-resource-groups-api-openapi.yml
  format: yaml
  label: Microsoft Azure Resource Groups API
  slug: azure-resource-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure/refs/heads/main/openapi/azure-resource-groups-api-openapi.yml
- filename: azure-resources-api-openapi.yml
  format: yaml
  label: Microsoft Azure Resources API
  slug: azure-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure/refs/heads/main/openapi/azure-resources-api-openapi.yml
- filename: azure-subscriptions-api-openapi.yml
  format: yaml
  label: Microsoft Azure Subscriptions API
  slug: azure-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure/refs/heads/main/openapi/azure-subscriptions-api-openapi.yml
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
- cert_expires: Jan  5 19:53:18 2027 GMT
  host: portal.azure.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 22:04:48 2026 GMT
  host: azure.microsoft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 23:36:21 2026 GMT
  host: management.azure.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Azure Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Azure, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Microsoft Azure
provider_slug: azure
slug: azure-domain-security
source_filename: azure-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: portal.azure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 19:53:18 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: azure.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 22:04:48 2026 GMT\n  hsts: null\n- host: management.azure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:36:21 2026 GMT\n  hsts: null\ndomains:\n- domain: azure.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure/refs/heads/main/security/azure-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Computing
- Databases
- Infrastructure
- Machine-Learning
- Networking
- Platform-as-a-Service
- Storage
---
