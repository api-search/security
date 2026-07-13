---
api_specs:
- filename: $metadata
  format: yaml
  label: Dynamics 365 Sales API
  slug: dynamics-365-sales-api
  spec_type: OpenAPI
  url: https://[org].api.crm.dynamics.com/api/data/v9.2/$metadata
- filename: $metadata
  format: yaml
  label: Dynamics 365 Customer Service API
  slug: dynamics-365-customer-service-api
  spec_type: OpenAPI
  url: https://[org].api.crm.dynamics.com/api/data/v9.2/$metadata
- filename: openapi
  format: yaml
  label: Dynamics 365 Business Central API
  slug: dynamics-365-business-central-api
  spec_type: OpenAPI
  url: https://docs.microsoft.com/dynamics365/business-central/dev-itpro/api-reference/v2.0/openapi
- filename: microsoft-dynamics-365-dataverse-web-api-openapi.yml
  format: yaml
  label: Microsoft Dataverse Web API
  slug: microsoft-dataverse-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365/refs/heads/main/openapi/microsoft-dynamics-365-dataverse-web-api-openapi.yml
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
- cert_expires: Dec 10 06:59:10 2026 GMT
  host: docs.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 28 08:57:28 2026 GMT
  host: api.businesscentral.dynamics.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microsoft Dynamics 365 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Dynamics 365, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Microsoft Dynamics 365
provider_slug: microsoft-dynamics-365
slug: microsoft-dynamics-365-domain-security
source_filename: microsoft-dynamics-365-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: portal.azure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 19:53:18 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 06:59:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.businesscentral.dynamics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 08:57:28 2026 GMT\n  hsts: null\ndomains:\n- domain: azure.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365/refs/heads/main/security/microsoft-dynamics-365-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Business Applications
- Cloud
- CRM
- Enterprise
- ERP
- Microsoft
---
