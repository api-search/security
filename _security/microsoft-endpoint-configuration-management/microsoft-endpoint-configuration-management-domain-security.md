---
api_specs:
- filename: microsoft-endpoint-configuration-management-configmgr-rest-api-openapi.yml
  format: yaml
  label: Configuration Manager REST API
  slug: configuration-manager-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-endpoint-configuration-management/refs/heads/main/openapi/microsoft-endpoint-configuration-management-configmgr-rest-api-openapi.yml
- filename: microsoft-endpoint-configuration-management-intune-graph-api-openapi.yml
  format: yaml
  label: Microsoft Intune Graph API
  slug: microsoft-intune-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-endpoint-configuration-management/refs/heads/main/openapi/microsoft-endpoint-configuration-management-intune-graph-api-openapi.yml
- filename: microsoft-endpoint-configuration-management-intune-data-warehouse-api-openapi.yml
  format: yaml
  label: Intune Data Warehouse API
  slug: intune-data-warehouse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-endpoint-configuration-management/refs/heads/main/openapi/microsoft-endpoint-configuration-management-intune-data-warehouse-api-openapi.yml
- filename: microsoft-endpoint-configuration-management-intune-reporting-export-api-openapi.yml
  format: yaml
  label: Intune Reporting Export API
  slug: intune-reporting-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-endpoint-configuration-management/refs/heads/main/openapi/microsoft-endpoint-configuration-management-intune-reporting-export-api-openapi.yml
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
- cert_expires: Dec 21 07:10:40 2026 GMT
  host: endpoint.microsoft.com
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
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: graph.microsoft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microsoft Endpoint Configuration Management Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Endpoint Configuration Management, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Endpoint Configuration Management
provider_slug: microsoft-endpoint-configuration-management
slug: microsoft-endpoint-configuration-management-domain-security
source_filename: microsoft-endpoint-configuration-management-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: endpoint.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 07:10:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: graph.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-endpoint-configuration-management/refs/heads/main/security/microsoft-endpoint-configuration-management-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Compliance
- Configuration Management
- Device Management
- Endpoint Management
- Mobile Device Management
- Patch Management
- Software Deployment
---
