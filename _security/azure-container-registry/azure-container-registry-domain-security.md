---
api_specs:
- filename: azure-container-registry-openapi.yaml
  format: yaml
  label: Azure Container Registry
  slug: azure-container-registry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/openapi/azure-container-registry-openapi.yaml
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
name: Azure Container Registry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Azure Container Registry, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Azure Container Registry
provider_slug: azure-container-registry
slug: azure-container-registry-domain-security
source_filename: azure-container-registry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: azure.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 22:04:48 2026 GMT\n  hsts: null\n- host: management.azure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:36:21 2026 GMT\n  hsts: null\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: azure.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/security/azure-container-registry-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
---
