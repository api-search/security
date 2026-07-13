---
api_specs:
- filename: microsoft-dynamics-business-central-openapi.yml
  format: yaml
  label: Microsoft Dynamics 365 Business Central API
  slug: business-central-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-business-central-openapi.yml
- filename: microsoft-dynamics-dataverse-openapi.yml
  format: yaml
  label: Microsoft Dynamics 365 Dataverse Web API
  slug: dataverse-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-dataverse-openapi.yml
- filename: microsoft-dynamics-finance-operations-openapi.yml
  format: yaml
  label: Microsoft Dynamics 365 Finance & Operations Data API
  slug: finance-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-finance-operations-openapi.yml
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
- cert_expires: Dec 11 02:26:09 2026 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microsoft Dynamics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Dynamics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Dynamics
provider_slug: microsoft-dynamics
slug: microsoft-dynamics-domain-security
source_filename: microsoft-dynamics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/security/microsoft-dynamics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CRM
- ERP
- Microsoft Dynamics
---
