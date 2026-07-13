---
api_specs:
- filename: microsoft-purview-catalog-openapi.yml
  format: yaml
  label: Microsoft Purview Catalog API
  slug: microsoft-purview-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-purview/refs/heads/main/openapi/microsoft-purview-catalog-openapi.yml
- filename: microsoft-purview-scanning-openapi.yml
  format: yaml
  label: Microsoft Purview Scanning API
  slug: microsoft-purview-scanning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-purview/refs/heads/main/openapi/microsoft-purview-scanning-openapi.yml
- filename: microsoft-purview-account-openapi.yml
  format: yaml
  label: Microsoft Purview Account API
  slug: microsoft-purview-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-purview/refs/heads/main/openapi/microsoft-purview-account-openapi.yml
- filename: microsoft-purview-data-map-openapi.yml
  format: yaml
  label: Microsoft Purview Data Map API
  slug: microsoft-purview-data-map-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-purview/refs/heads/main/openapi/microsoft-purview-data-map-openapi.yml
- filename: microsoft-purview-metadata-policies-openapi.yml
  format: yaml
  label: Microsoft Purview Metadata Policies API
  slug: microsoft-purview-metadata-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-purview/refs/heads/main/openapi/microsoft-purview-metadata-policies-openapi.yml
- filename: microsoft-purview-workflow-openapi.yml
  format: yaml
  label: Microsoft Purview Workflow API
  slug: microsoft-purview-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-purview/refs/heads/main/openapi/microsoft-purview-workflow-openapi.yml
- filename: microsoft-purview-unified-catalog-openapi.yml
  format: yaml
  label: Microsoft Purview Unified Catalog API
  slug: microsoft-purview-unified-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-purview/refs/heads/main/openapi/microsoft-purview-unified-catalog-openapi.yml
- filename: microsoft-purview-data-quality-openapi.yml
  format: yaml
  label: Microsoft Purview Data Quality API
  slug: microsoft-purview-data-quality-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-purview/refs/heads/main/openapi/microsoft-purview-data-quality-openapi.yml
- filename: microsoft-purview-ediscovery-openapi.yml
  format: yaml
  label: Microsoft Purview eDiscovery API
  slug: microsoft-purview-ediscovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-purview/refs/heads/main/openapi/microsoft-purview-ediscovery-openapi.yml
- filename: microsoft-purview-information-protection-openapi.yml
  format: yaml
  label: Microsoft Purview Information Protection API
  slug: microsoft-purview-information-protection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-purview/refs/heads/main/openapi/microsoft-purview-information-protection-openapi.yml
- filename: microsoft-purview-data-security-governance-openapi.yml
  format: yaml
  label: Microsoft Purview Data Security and Governance API
  slug: microsoft-purview-data-security-and-governance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-purview/refs/heads/main/openapi/microsoft-purview-data-security-governance-openapi.yml
- filename: microsoft-purview-records-management-openapi.yml
  format: yaml
  label: Microsoft Purview Records Management API
  slug: microsoft-purview-records-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-purview/refs/heads/main/openapi/microsoft-purview-records-management-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Nov  6 23:03:08 2026 GMT
  host: purview.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 17 19:55:21 2027 GMT
  host: www.microsoft.com
  hsts: false
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
name: Microsoft Purview Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Purview, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Purview
provider_slug: microsoft-purview
slug: microsoft-purview-domain-security
source_filename: microsoft-purview-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: purview.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:03:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 19:55:21 2027 GMT\n  hsts: false\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-purview/refs/heads/main/security/microsoft-purview-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Compliance
- Data Catalog
- Data Classification
- Data Governance
- Data Loss Prevention
- Information Protection
---
