---
api_specs:
- filename: qubiqle-accounts-api-openapi.yml
  format: yaml
  label: Qubiqle accounts API
  slug: qubiqle-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qubiqle/refs/heads/main/openapi/qubiqle-accounts-api-openapi.yml
- filename: qubiqle-batch-api-openapi.yml
  format: yaml
  label: Qubiqle batch API
  slug: qubiqle-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qubiqle/refs/heads/main/openapi/qubiqle-batch-api-openapi.yml
- filename: qubiqle-catalog-api-openapi.yml
  format: yaml
  label: Qubiqle catalog API
  slug: qubiqle-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qubiqle/refs/heads/main/openapi/qubiqle-catalog-api-openapi.yml
- filename: qubiqle-dimensions-api-openapi.yml
  format: yaml
  label: Qubiqle dimensions API
  slug: qubiqle-dimensions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qubiqle/refs/heads/main/openapi/qubiqle-dimensions-api-openapi.yml
- filename: qubiqle-invoices-api-openapi.yml
  format: yaml
  label: Qubiqle invoices API
  slug: qubiqle-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qubiqle/refs/heads/main/openapi/qubiqle-invoices-api-openapi.yml
- filename: qubiqle-oauth-api-openapi.yml
  format: yaml
  label: Qubiqle oauth API
  slug: qubiqle-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qubiqle/refs/heads/main/openapi/qubiqle-oauth-api-openapi.yml
- filename: qubiqle-purchaseorders-api-openapi.yml
  format: yaml
  label: Qubiqle purchaseOrders API
  slug: qubiqle-purchaseorders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qubiqle/refs/heads/main/openapi/qubiqle-purchaseorders-api-openapi.yml
- filename: qubiqle-receipts-api-openapi.yml
  format: yaml
  label: Qubiqle receipts API
  slug: qubiqle-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qubiqle/refs/heads/main/openapi/qubiqle-receipts-api-openapi.yml
- filename: qubiqle-vendors-api-openapi.yml
  format: yaml
  label: Qubiqle vendors API
  slug: qubiqle-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qubiqle/refs/heads/main/openapi/qubiqle-vendors-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ottimate.com
  spf: true
hosts:
- cert_expires: Oct 12 23:12:52 2026 GMT
  host: ottimate.com
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
name: Qubiqle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qubiqle, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Qubiqle
provider_slug: qubiqle
slug: qubiqle-domain-security
source_filename: qubiqle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ottimate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 23:12:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.ottimate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 01:01:08 2026 GMT\n  hsts: null\n- host: sandbox-api.ottimate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 18:31:18 2026 GMT\n  hsts: null\ndomains:\n- domain: ottimate.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qubiqle/refs/heads/main/security/qubiqle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Accounts Payable
- Invoicing
- Payments
- Accounting
- FinTech
- Automation
- Artificial Intelligence
- ERP Integration
- Procurement
---
