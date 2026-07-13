---
api_specs:
- filename: dynamics-open-api
  format: yaml
  label: Business Central API (v2.0)
  slug: api-v2
  spec_type: OpenAPI
  url: https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/api-reference/v2.0/dynamics-open-api
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
- Operations
- Small Business
- Mid-Market
- Microsoft Dynamics 365
---
