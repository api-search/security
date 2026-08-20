---
api_specs:
- filename: plateiq-accounts-api-openapi.yml
  format: yaml
  label: PlateIQ accounts API
  slug: plateiq-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plateiq/refs/heads/main/openapi/plateiq-accounts-api-openapi.yml
- filename: plateiq-batch-api-openapi.yml
  format: yaml
  label: PlateIQ batch API
  slug: plateiq-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plateiq/refs/heads/main/openapi/plateiq-batch-api-openapi.yml
- filename: plateiq-catalog-api-openapi.yml
  format: yaml
  label: PlateIQ catalog API
  slug: plateiq-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plateiq/refs/heads/main/openapi/plateiq-catalog-api-openapi.yml
- filename: plateiq-dimensions-api-openapi.yml
  format: yaml
  label: PlateIQ dimensions API
  slug: plateiq-dimensions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plateiq/refs/heads/main/openapi/plateiq-dimensions-api-openapi.yml
- filename: plateiq-invoices-api-openapi.yml
  format: yaml
  label: PlateIQ invoices API
  slug: plateiq-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plateiq/refs/heads/main/openapi/plateiq-invoices-api-openapi.yml
- filename: plateiq-oauth-api-openapi.yml
  format: yaml
  label: PlateIQ oauth API
  slug: plateiq-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plateiq/refs/heads/main/openapi/plateiq-oauth-api-openapi.yml
- filename: plateiq-purchaseorders-api-openapi.yml
  format: yaml
  label: PlateIQ purchaseOrders API
  slug: plateiq-purchaseorders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plateiq/refs/heads/main/openapi/plateiq-purchaseorders-api-openapi.yml
- filename: plateiq-receipts-api-openapi.yml
  format: yaml
  label: PlateIQ receipts API
  slug: plateiq-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plateiq/refs/heads/main/openapi/plateiq-receipts-api-openapi.yml
- filename: plateiq-vendors-api-openapi.yml
  format: yaml
  label: PlateIQ vendors API
  slug: plateiq-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plateiq/refs/heads/main/openapi/plateiq-vendors-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: plateiq.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ottimate.com
  spf: true
hosts:
- cert_expires: Sep 23 15:20:12 2026 GMT
  host: plateiq.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 01:01:08 2026 GMT
  host: api.ottimate.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 18:31:18 2026 GMT
  host: sandbox-api.ottimate.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Plateiq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PlateIQ, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PlateIQ
provider_slug: plateiq
slug: plateiq-domain-security
source_filename: plateiq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: plateiq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 15:20:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.ottimate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 01:01:08 2026 GMT\n  hsts: null\n- host: sandbox-api.ottimate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 18:31:18 2026 GMT\n  hsts: null\ndomains:\n- domain: plateiq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: ottimate.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plateiq/refs/heads/main/security/plateiq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise Saas
- Accounts Payable
- Invoice Automation
- Payments
- Fintech
- Restaurant
- Procurement
- Spend Management
- ERP Integration
---
