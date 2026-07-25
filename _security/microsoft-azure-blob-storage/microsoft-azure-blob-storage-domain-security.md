---
api_specs:
- filename: microsoft-azure-blob-storage-append-blobs-api-openapi.yml
  format: yaml
  label: Azure Blob Storage Append Blobs API
  slug: microsoft-azure-blob-storage-append-blobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-blob-storage/refs/heads/main/openapi/microsoft-azure-blob-storage-append-blobs-api-openapi.yml
- filename: microsoft-azure-blob-storage-azure-blob-storage-rest-api-api-openapi.yml
  format: yaml
  label: Azure Blob Storage Azure Blob Storage REST API API
  slug: microsoft-azure-blob-storage-azure-blob-storage-rest-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-blob-storage/refs/heads/main/openapi/microsoft-azure-blob-storage-azure-blob-storage-rest-api-api-openapi.yml
- filename: microsoft-azure-blob-storage-blobs-api-openapi.yml
  format: yaml
  label: Azure Blob Storage Blobs API
  slug: microsoft-azure-blob-storage-blobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-blob-storage/refs/heads/main/openapi/microsoft-azure-blob-storage-blobs-api-openapi.yml
- filename: microsoft-azure-blob-storage-block-blobs-api-openapi.yml
  format: yaml
  label: Azure Blob Storage Block Blobs API
  slug: microsoft-azure-blob-storage-block-blobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-blob-storage/refs/heads/main/openapi/microsoft-azure-blob-storage-block-blobs-api-openapi.yml
- filename: microsoft-azure-blob-storage-comp-blobs-api-openapi.yml
  format: yaml
  label: Azure Blob Storage ?comp=blobs API
  slug: microsoft-azure-blob-storage-comp-blobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-blob-storage/refs/heads/main/openapi/microsoft-azure-blob-storage-comp-blobs-api-openapi.yml
- filename: microsoft-azure-blob-storage-containers-api-openapi.yml
  format: yaml
  label: Azure Blob Storage Containers API
  slug: microsoft-azure-blob-storage-containers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-blob-storage/refs/heads/main/openapi/microsoft-azure-blob-storage-containers-api-openapi.yml
- filename: microsoft-azure-blob-storage-page-blobs-api-openapi.yml
  format: yaml
  label: Azure Blob Storage Page Blobs API
  slug: microsoft-azure-blob-storage-page-blobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-blob-storage/refs/heads/main/openapi/microsoft-azure-blob-storage-page-blobs-api-openapi.yml
- filename: microsoft-azure-blob-storage-restype-service-comp-batch-api-openapi.yml
  format: yaml
  label: Azure Blob Storage ?restype=service&comp=batch API
  slug: microsoft-azure-blob-storage-restype-service-comp-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-blob-storage/refs/heads/main/openapi/microsoft-azure-blob-storage-restype-service-comp-batch-api-openapi.yml
- filename: microsoft-azure-blob-storage-restype-service-comp-properties-api-openapi.yml
  format: yaml
  label: Azure Blob Storage ?restype=service&comp=properties API
  slug: microsoft-azure-blob-storage-restype-service-comp-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-blob-storage/refs/heads/main/openapi/microsoft-azure-blob-storage-restype-service-comp-properties-api-openapi.yml
- filename: microsoft-azure-blob-storage-restype-service-comp-stats-api-openapi.yml
  format: yaml
  label: Azure Blob Storage ?restype=service&comp=stats API
  slug: microsoft-azure-blob-storage-restype-service-comp-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-blob-storage/refs/heads/main/openapi/microsoft-azure-blob-storage-restype-service-comp-stats-api-openapi.yml
- filename: microsoft-azure-blob-storage-restype-service-comp-userdelegationkey-api-openapi.yml
  format: yaml
  label: Azure Blob Storage ?restype=service&comp=userdelegationkey API
  slug: microsoft-azure-blob-storage-restype-service-comp-userdelegationkey-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-blob-storage/refs/heads/main/openapi/microsoft-azure-blob-storage-restype-service-comp-userdelegationkey-api-openapi.yml
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
- cert_expires: Dec 11 02:26:09 2026 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microsoft Azure Blob Storage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Azure Blob Storage, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Azure Blob Storage
provider_slug: microsoft-azure-blob-storage
slug: microsoft-azure-blob-storage-domain-security
source_filename: microsoft-azure-blob-storage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: portal.azure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 19:53:18 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: azure.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 22:04:48 2026 GMT\n  hsts: null\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: azure.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-blob-storage/refs/heads/main/security/microsoft-azure-blob-storage-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Azure
- Blobs
- Cloud Storage
- Microsoft
- Object Storage
- Storage
---
