---
api_specs:
- filename: microsoft-azure-api-management-rest-api-openapi.yaml
  format: yaml
  label: Azure API Management REST API
  slug: azure-api-management-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-api-management/refs/heads/main/openapi/microsoft-azure-api-management-rest-api-openapi.yaml
- filename: microsoft-azure-api-management-gateway-openapi.yaml
  format: yaml
  label: Azure API Management Gateway
  slug: azure-api-management-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-api-management/refs/heads/main/openapi/microsoft-azure-api-management-gateway-openapi.yaml
- filename: microsoft-azure-api-management-self-hosted-gateway-openapi.yaml
  format: yaml
  label: Azure API Management Self-Hosted Gateway
  slug: azure-api-management-self-hosted-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-api-management/refs/heads/main/openapi/microsoft-azure-api-management-self-hosted-gateway-openapi.yaml
- filename: microsoft-azure-api-management-ai-gateway-openapi.yaml
  format: yaml
  label: Azure API Management AI Gateway
  slug: azure-api-management-ai-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-api-management/refs/heads/main/openapi/microsoft-azure-api-management-ai-gateway-openapi.yaml
- filename: microsoft-azure-api-management-developer-portal-openapi.yaml
  format: yaml
  label: Azure API Management Developer Portal
  slug: azure-api-management-developer-portal
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-api-management/refs/heads/main/openapi/microsoft-azure-api-management-developer-portal-openapi.yaml
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
name: Microsoft Azure Api Management Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Azure API Management, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Azure API Management
provider_slug: microsoft-azure-api-management
slug: microsoft-azure-api-management-domain-security
source_filename: microsoft-azure-api-management-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: azure.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 22:04:48 2026 GMT\n  hsts: null\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: management.azure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:36:21 2026 GMT\n  hsts: null\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: azure.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-api-management/refs/heads/main/security/microsoft-azure-api-management-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- A2A
- AI Gateway
- API Center
- API Gateway
- API Management
- Enterprise
- MCP
- Microsoft Azure
---
