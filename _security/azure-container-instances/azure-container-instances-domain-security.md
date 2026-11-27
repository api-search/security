---
api_specs:
- filename: azure-container-instances-operations-api-openapi.yml
  format: yaml
  label: Azure Container Instances Operations API
  slug: azure-container-instances-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-container-instances/openapi/azure-container-instances-operations-api-openapi.yml
- filename: azure-container-instances-subscriptions-api-openapi.yml
  format: yaml
  label: Azure Container Instances Subscriptions API
  slug: azure-container-instances-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-container-instances/openapi/azure-container-instances-subscriptions-api-openapi.yml
- filename: azure-container-instances-sandboxgroups-api-openapi.yml
  format: yaml
  label: Azure Container Instances Sandbox Groups API
  slug: azure-container-instances-sandboxgroups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-container-instances/openapi/azure-container-instances-sandboxgroups-api-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
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
- cert_expires: Jan 21 18:52:15 2027 GMT
  host: portal.azure.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  2 19:05:38 2027 GMT
  host: azure.microsoft.com
  hsts: null
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
name: Azure Container Instances Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Azure Container Instances, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Azure Container Instances
provider_slug: azure-container-instances
slug: azure-container-instances-domain-security
source_filename: azure-container-instances-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: portal.azure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 18:52:15 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: azure.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  2 19:05:38 2027 GMT\n  hsts: null\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  8 00:23:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: azure.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/azure-container-instances/security/azure-container-instances-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Microsoft Azure
- Cloud
- Container Instances
- Containers
- Microsoft
- Serverless
---
