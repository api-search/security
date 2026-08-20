---
api_specs:
- filename: microsoft-dynamics-365-business-central-companies-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics 365 Business Central Companies API
  slug: microsoft-dynamics-365-business-central-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365-business-central/refs/heads/main/openapi/microsoft-dynamics-365-business-central-companies-api-openapi.yml
- filename: microsoft-dynamics-365-business-central-customers-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics 365 Business Central Customers API
  slug: microsoft-dynamics-365-business-central-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365-business-central/refs/heads/main/openapi/microsoft-dynamics-365-business-central-customers-api-openapi.yml
- filename: microsoft-dynamics-365-business-central-items-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics 365 Business Central Items API
  slug: microsoft-dynamics-365-business-central-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365-business-central/refs/heads/main/openapi/microsoft-dynamics-365-business-central-items-api-openapi.yml
- filename: microsoft-dynamics-365-business-central-purchaseorders-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics 365 Business Central PurchaseOrders API
  slug: microsoft-dynamics-365-business-central-purchaseorders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365-business-central/refs/heads/main/openapi/microsoft-dynamics-365-business-central-purchaseorders-api-openapi.yml
- filename: microsoft-dynamics-365-business-central-salesinvoices-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics 365 Business Central SalesInvoices API
  slug: microsoft-dynamics-365-business-central-salesinvoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365-business-central/refs/heads/main/openapi/microsoft-dynamics-365-business-central-salesinvoices-api-openapi.yml
- filename: microsoft-dynamics-365-business-central-salesorders-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics 365 Business Central SalesOrders API
  slug: microsoft-dynamics-365-business-central-salesorders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365-business-central/refs/heads/main/openapi/microsoft-dynamics-365-business-central-salesorders-api-openapi.yml
- filename: microsoft-dynamics-365-business-central-vendors-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics 365 Business Central Vendors API
  slug: microsoft-dynamics-365-business-central-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365-business-central/refs/heads/main/openapi/microsoft-dynamics-365-business-central-vendors-api-openapi.yml
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
  dmarc_policy: reject
  dnssec: false
  domain: dynamics.com
  spf: false
hosts:
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
- cert_expires: Dec 28 08:57:28 2026 GMT
  host: api.businesscentral.dynamics.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microsoft Dynamics 365 Business Central Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Dynamics 365 Business Central, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Dynamics 365 Business Central
provider_slug: microsoft-dynamics-365-business-central
slug: microsoft-dynamics-365-business-central-domain-security
source_filename: microsoft-dynamics-365-business-central-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 19:55:21 2027 GMT\n  hsts: false\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.businesscentral.dynamics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 08:57:28 2026 GMT\n  hsts: null\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: dynamics.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365-business-central/refs/heads/main/security/microsoft-dynamics-365-business-central-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- ERP
- Cloud ERP
- Finance
- Accounting
- Supply Chain
- Small Business
- Mid-Market
- Microsoft Dynamics 365
---
