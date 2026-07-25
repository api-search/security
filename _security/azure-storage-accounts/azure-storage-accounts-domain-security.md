---
api_specs:
- filename: azure-storage-accounts-blobcontainers-api-openapi.yml
  format: yaml
  label: Azure Storage Accounts BlobContainers API
  slug: azure-storage-accounts-blobcontainers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/openapi/azure-storage-accounts-blobcontainers-api-openapi.yml
- filename: azure-storage-accounts-blobservice-api-openapi.yml
  format: yaml
  label: Azure Storage Accounts BlobService API
  slug: azure-storage-accounts-blobservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/openapi/azure-storage-accounts-blobservice-api-openapi.yml
- filename: azure-storage-accounts-locationusage-api-openapi.yml
  format: yaml
  label: Azure Storage Accounts LocationUsage API
  slug: azure-storage-accounts-locationusage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/openapi/azure-storage-accounts-locationusage-api-openapi.yml
- filename: azure-storage-accounts-managementpolicies-api-openapi.yml
  format: yaml
  label: Azure Storage Accounts ManagementPolicies API
  slug: azure-storage-accounts-managementpolicies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/openapi/azure-storage-accounts-managementpolicies-api-openapi.yml
- filename: azure-storage-accounts-operations-api-openapi.yml
  format: yaml
  label: Azure Storage Accounts Operations API
  slug: azure-storage-accounts-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/openapi/azure-storage-accounts-operations-api-openapi.yml
- filename: azure-storage-accounts-privateendpointconnections-api-openapi.yml
  format: yaml
  label: Azure Storage Accounts PrivateEndpointConnections API
  slug: azure-storage-accounts-privateendpointconnections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/openapi/azure-storage-accounts-privateendpointconnections-api-openapi.yml
- filename: azure-storage-accounts-privatelinkresources-api-openapi.yml
  format: yaml
  label: Azure Storage Accounts PrivateLinkResources API
  slug: azure-storage-accounts-privatelinkresources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/openapi/azure-storage-accounts-privatelinkresources-api-openapi.yml
- filename: azure-storage-accounts-skus-api-openapi.yml
  format: yaml
  label: Azure Storage Accounts Skus API
  slug: azure-storage-accounts-skus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/openapi/azure-storage-accounts-skus-api-openapi.yml
- filename: azure-storage-accounts-storageaccounts-api-openapi.yml
  format: yaml
  label: Azure Storage Accounts StorageAccounts API
  slug: azure-storage-accounts-storageaccounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/openapi/azure-storage-accounts-storageaccounts-api-openapi.yml
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
- cert_expires: Dec 11 02:26:09 2026 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
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
name: Azure Storage Accounts Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Azure Storage Accounts, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
slug: azure-storage-accounts-domain-security
source_filename: azure-storage-accounts-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: portal.azure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 19:53:18 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: management.azure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:36:21 2026 GMT\n  hsts: null\ndomains:\n- domain: azure.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/security/azure-storage-accounts-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
---
