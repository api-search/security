---
api_specs:
- filename: azure-file-storage-account-api-openapi.yml
  format: yaml
  label: Azure Files Account API
  slug: azure-file-storage-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-file-storage/openapi/azure-file-storage-account-api-openapi.yml
- filename: azure-file-storage-directories-api-openapi.yml
  format: yaml
  label: Azure Files Directories API
  slug: azure-file-storage-directories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-file-storage/openapi/azure-file-storage-directories-api-openapi.yml
- filename: azure-file-storage-files-api-openapi.yml
  format: yaml
  label: Azure Files API
  slug: azure-file-storage-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-file-storage/openapi/azure-file-storage-files-api-openapi.yml
- filename: azure-file-storage-shares-api-openapi.yml
  format: yaml
  label: Azure Files Shares API
  slug: azure-file-storage-shares-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-file-storage/openapi/azure-file-storage-shares-api-openapi.yml
- filename: azure-file-storage-shares-api-openapi.yml
  format: yaml
  label: Azure File Storage Shares API
  slug: microsoft-azure-file-storage-shares-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-file-storage/openapi/azure-file-storage-shares-api-openapi.yml
- filename: azure-file-storage-directory-api-openapi.yml
  format: yaml
  label: Azure Files Directory API
  slug: azure-file-storage-directory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-file-storage/openapi/azure-file-storage-directory-api-openapi.yml
- filename: azure-file-storage-file-api-openapi.yml
  format: yaml
  label: Azure Files File API
  slug: azure-file-storage-file-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-file-storage/openapi/azure-file-storage-file-api-openapi.yml
- filename: azure-file-storage-service-api-openapi.yml
  format: yaml
  label: Azure Files Service API
  slug: azure-file-storage-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-file-storage/openapi/azure-file-storage-service-api-openapi.yml
- filename: azure-file-storage-share-api-openapi.yml
  format: yaml
  label: Azure Files Share API
  slug: azure-file-storage-share-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-file-storage/openapi/azure-file-storage-share-api-openapi.yml
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
name: Azure File Storage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Azure Files, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Azure Files
provider_slug: azure-file-storage
slug: azure-file-storage-domain-security
source_filename: azure-file-storage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: portal.azure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 18:52:15 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: azure.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  2 19:05:38 2027 GMT\n  hsts: null\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  8 00:23:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: azure.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/azure-file-storage/security/azure-file-storage-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Storage
- File Storage
- File Shares
- NFS
- Cloud
- Microsoft Azure
- Server Message Block
---
