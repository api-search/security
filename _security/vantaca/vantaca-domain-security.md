---
api_specs:
- filename: vantaca-openapi.json
  format: json
  label: Vantaca Associations API
  slug: vantaca-associations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantaca/refs/heads/main/openapi/vantaca-openapi.json
- filename: vantaca-openapi.json
  format: json
  label: Vantaca Homeowner Accounts API
  slug: vantaca-homeowner-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantaca/refs/heads/main/openapi/vantaca-openapi.json
- filename: vantaca-openapi.json
  format: json
  label: Vantaca Accounts Payable & Ledger API
  slug: vantaca-accounts-payable-ledger-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantaca/refs/heads/main/openapi/vantaca-openapi.json
- filename: vantaca-openapi.json
  format: json
  label: Vantaca Work Orders API
  slug: vantaca-work-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantaca/refs/heads/main/openapi/vantaca-openapi.json
- filename: vantaca-openapi.json
  format: json
  label: Vantaca Violations & Compliance API
  slug: vantaca-violations-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantaca/refs/heads/main/openapi/vantaca-openapi.json
- filename: vantaca-openapi.json
  format: json
  label: Vantaca Architectural Requests (ARC) API
  slug: vantaca-architectural-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantaca/refs/heads/main/openapi/vantaca-openapi.json
- filename: vantaca-openapi.json
  format: json
  label: Vantaca Vendors & Service Providers API
  slug: vantaca-vendors-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantaca/refs/heads/main/openapi/vantaca-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vantaca.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: swaggerhub.com
  spf: true
hosts:
- cert_expires: Sep  6 12:43:07 2026 GMT
  host: www.vantaca.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: app.swaggerhub.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 23 19:01:47 2027 GMT
  host: api.vantaca.net
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Vantaca Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vantaca, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Vantaca
provider_slug: vantaca
slug: vantaca-domain-security
source_filename: vantaca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vantaca.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 12:43:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.swaggerhub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: null\n- host: api.vantaca.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 23 19:01:47 2027 GMT\n  hsts: false\ndomains:\n- domain: vantaca.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: swaggerhub.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vantaca/refs/heads/main/security/vantaca-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- HOA
- Community Association Management
- CAM
- Property Management
- Real Estate
- Accounting
- Workflow Automation
- Vendor Management
---
