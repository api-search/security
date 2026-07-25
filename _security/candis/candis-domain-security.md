---
api_specs:
- filename: candis-core-data-api-openapi.yml
  format: yaml
  label: Candis Core Data API
  slug: candis-core-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candis/refs/heads/main/openapi/candis-core-data-api-openapi.yml
- filename: candis-exports-api-openapi.yml
  format: yaml
  label: Candis Exports API
  slug: candis-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candis/refs/heads/main/openapi/candis-exports-api-openapi.yml
- filename: candis-invoices-api-openapi.yml
  format: yaml
  label: Candis Invoices API
  slug: candis-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candis/refs/heads/main/openapi/candis-invoices-api-openapi.yml
- filename: candis-organizations-api-openapi.yml
  format: yaml
  label: Candis Organizations API
  slug: candis-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candis/refs/heads/main/openapi/candis-organizations-api-openapi.yml
- filename: candis-purchase-requests-api-openapi.yml
  format: yaml
  label: Candis Purchase Requests API
  slug: candis-purchase-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candis/refs/heads/main/openapi/candis-purchase-requests-api-openapi.yml
- filename: candis-reimbursements-api-openapi.yml
  format: yaml
  label: Candis Reimbursements API
  slug: candis-reimbursements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candis/refs/heads/main/openapi/candis-reimbursements-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: candis.io
  spf: true
hosts:
- cert_expires: Sep 15 06:11:28 2026 GMT
  host: www.candis.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Candis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Candis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Candis
provider_slug: candis
slug: candis-domain-security
source_filename: candis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.candis.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 06:11:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: candis.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/candis/refs/heads/main/security/candis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Accounts Payable
- Spend Management
- Invoice Management
- Financial Process Automation
- Accounting
- DATEV
- OCR
- Germany
---
