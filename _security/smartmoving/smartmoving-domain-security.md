---
api_specs:
- filename: smartmoving-openapi.yml
  format: yaml
  label: SmartMoving Customers API
  slug: smartmoving-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartmoving/refs/heads/main/openapi/smartmoving-openapi.yml
- filename: smartmoving-openapi.yml
  format: yaml
  label: SmartMoving Opportunities API
  slug: smartmoving-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartmoving/refs/heads/main/openapi/smartmoving-openapi.yml
- filename: smartmoving-openapi.yml
  format: yaml
  label: SmartMoving Leads API
  slug: smartmoving-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartmoving/refs/heads/main/openapi/smartmoving-openapi.yml
- filename: smartmoving-openapi.yml
  format: yaml
  label: SmartMoving Lead Provider API
  slug: smartmoving-lead-provider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartmoving/refs/heads/main/openapi/smartmoving-openapi.yml
- filename: smartmoving-openapi.yml
  format: yaml
  label: SmartMoving Jobs & Moves API
  slug: smartmoving-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartmoving/refs/heads/main/openapi/smartmoving-openapi.yml
- filename: smartmoving-openapi.yml
  format: yaml
  label: SmartMoving Reference Data API
  slug: smartmoving-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartmoving/refs/heads/main/openapi/smartmoving-openapi.yml
- filename: smartmoving-openapi.yml
  format: yaml
  label: SmartMoving Webhooks API
  slug: smartmoving-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartmoving/refs/heads/main/openapi/smartmoving-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: smartmoving.com
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: false
  dnssec: false
  domain: azure-api.net
  spf: false
hosts:
- cert_expires: Sep 10 23:18:33 2026 GMT
  host: www.smartmoving.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 08:10:36 2026 GMT
  host: smartmoving-prod-api-management.developer.azure-api.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: api.smartmoving.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Smartmoving Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SmartMoving, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SmartMoving
provider_slug: smartmoving
slug: smartmoving-domain-security
source_filename: smartmoving-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.smartmoving.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:18:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: smartmoving-prod-api-management.developer.azure-api.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 08:10:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.smartmoving.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: smartmoving.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: azure-api.net\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smartmoving/refs/heads/main/security/smartmoving-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Moving Software
- CRM
- Field Service
- Moving Company
- Operations
- Lead Management
- Dispatch
---
