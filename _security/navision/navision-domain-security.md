---
api_specs:
- filename: nav-webservices.yaml
  format: yaml
  label: Dynamics NAV Web Services API
  slug: dynamics-nav-web-services-api
  spec_type: OpenAPI
  url: https://example.com/openapi/nav-webservices.yaml
- filename: nav-odata.yaml
  format: yaml
  label: Dynamics NAV OData API
  slug: dynamics-nav-odata-api
  spec_type: OpenAPI
  url: https://example.com/openapi/nav-odata.yaml
- filename: business-central-api-v2.yml
  format: yaml
  label: Business Central API v2.0
  slug: business-central-api-v20
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/openapi/business-central-api-v2.yml
- filename: admin-center-api.yml
  format: yaml
  label: Business Central Administration Center API
  slug: business-central-administration-center-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/openapi/admin-center-api.yml
- filename: automation-api.yml
  format: yaml
  label: Business Central Automation API
  slug: business-central-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/openapi/automation-api.yml
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
- cert_expires: Dec 20 09:04:17 2026 GMT
  host: dynamics.microsoft.com
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
- cert_expires: Dec 28 08:57:28 2026 GMT
  host: api.businesscentral.dynamics.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Navision Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Dynamics NAV, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Dynamics NAV
provider_slug: navision
slug: navision-domain-security
source_filename: navision-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dynamics.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 09:04:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.businesscentral.dynamics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 08:57:28 2026 GMT\n  hsts: null\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: dynamics.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/security/navision-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
---
