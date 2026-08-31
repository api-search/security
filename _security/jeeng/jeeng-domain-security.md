---
api_specs:
- filename: jeeng-management-api-openapi.yml
  format: yaml
  label: Jeeng Management API
  slug: jeeng-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jeeng/refs/heads/main/openapi/jeeng-management-api-openapi.yml
- filename: jeeng-reporting-api-openapi.yml
  format: yaml
  label: Jeeng Reporting API
  slug: jeeng-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jeeng/refs/heads/main/openapi/jeeng-reporting-api-openapi.yml
- filename: jeeng-revenuestripe-onmicrosoft-com-api-openapi.yml
  format: yaml
  label: Jeeng Revenuestripe.onmicrosoft.com API
  slug: jeeng-revenuestripe-onmicrosoft-com-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jeeng/refs/heads/main/openapi/jeeng-revenuestripe-onmicrosoft-com-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jeeng.com
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: false
  dnssec: false
  domain: azure-api.net
  spf: false
hosts:
- cert_expires: Sep 26 03:48:41 2026 GMT
  host: jeeng.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 07:01:37 2026 GMT
  host: developers.jeeng.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 11:23:56 2026 GMT
  host: powerinbox.azure-api.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jeeng Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jeeng, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Jeeng
provider_slug: jeeng
slug: jeeng-domain-security
source_filename: jeeng-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jeeng.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 03:48:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.jeeng.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 07:01:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: powerinbox.azure-api.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 11:23:56 2026 GMT\n  hsts: null\ndomains:\n- domain: jeeng.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: azure-api.net\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jeeng/refs/heads/main/security/jeeng-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- Publishing
- Email
- Push Notifications
- Monetization
- AdTech
- Newsletters
- Audience Engagement
- Reporting
- Analytics
- OData
- Authentication
---
