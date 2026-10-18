---
api_specs:
- filename: concur-expense-reports-api-openapi.yml
  format: yaml
  label: SAP Concur Expense Reports API
  slug: concur-expense-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/concur-expense-reports-api-openapi.yml
- filename: concur-expenses-api-openapi.yml
  format: yaml
  label: SAP Concur Expenses API
  slug: concur-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/concur-expenses-api-openapi.yml
- filename: concur-allocations-api-openapi.yml
  format: yaml
  label: SAP Concur Allocations API
  slug: concur-allocations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/concur-allocations-api-openapi.yml
- filename: concur-comments-api-openapi.yml
  format: yaml
  label: SAP Concur Comments API
  slug: concur-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/concur-comments-api-openapi.yml
- filename: concur-expense-entries-api-openapi.yml
  format: yaml
  label: SAP Concur Expense Entries API
  slug: concur-expense-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/concur-expense-entries-api-openapi.yml
- filename: concur-group-configurations-api-openapi.yml
  format: yaml
  label: SAP Concur Group Configurations API
  slug: concur-group-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/concur-group-configurations-api-openapi.yml
- filename: concur-payment-batches-api-openapi.yml
  format: yaml
  label: SAP Concur Payment Batches API
  slug: concur-payment-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/concur-payment-batches-api-openapi.yml
- filename: concur-quick-expenses-api-openapi.yml
  format: yaml
  label: SAP Concur Quick Expenses API
  slug: concur-quick-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/concur-quick-expenses-api-openapi.yml
- filename: concur-receipt-images-api-openapi.yml
  format: yaml
  label: SAP Concur Receipt Images API
  slug: concur-receipt-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/concur-receipt-images-api-openapi.yml
- filename: concur-reports-api-openapi.yml
  format: yaml
  label: SAP Concur Reports API
  slug: concur-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/concur-reports-api-openapi.yml
- filename: concur-workflows-api-openapi.yml
  format: yaml
  label: SAP Concur Workflows API
  slug: concur-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/concur-workflows-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: concur.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: concursolutions.com
  spf: true
hosts:
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: developer.concur.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: us.api.concursolutions.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: emea.api.concursolutions.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Concur Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SAP Concur, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: SAP Concur
provider_slug: concur
slug: concur-domain-security
source_filename: concur-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.concur.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: false\n- host: us.api.concursolutions.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: null\n- host: emea.api.concursolutions.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: concur.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: concursolutions.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/security/concur-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Expense Management
- Finance
- Invoices
- SAP
- Travel
- Business Travel
- Financial Services
- Invoice Management
- Travel Management
- Financial Management
- Receipts
- Reimbursement
- Reporting
---
