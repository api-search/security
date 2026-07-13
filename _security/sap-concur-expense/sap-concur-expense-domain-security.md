---
api_specs:
- filename: sap-concur-expense-report-openapi.yml
  format: yaml
  label: Expense Report v3 API
  slug: expense-report-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-concur-expense/refs/heads/main/openapi/sap-concur-expense-report-openapi.yml
- filename: sap-concur-expense-report-openapi.yml
  format: yaml
  label: Expense Entry v3 API
  slug: expense-entry-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-concur-expense/refs/heads/main/openapi/sap-concur-expense-report-openapi.yml
- filename: sap-concur-expense-report-openapi.yml
  format: yaml
  label: Quick Expense v3 API
  slug: quick-expense-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-concur-expense/refs/heads/main/openapi/sap-concur-expense-report-openapi.yml
- filename: sap-concur-expense-report-openapi.yml
  format: yaml
  label: Receipt Image v3 API
  slug: receipt-image-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-concur-expense/refs/heads/main/openapi/sap-concur-expense-report-openapi.yml
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
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: www.concur.com
  hsts: false
  https: true
  tls_version: TLSv1.3
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
kind: domain-security
layout: security
method: probed
name: Sap Concur Expense Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SAP Concur Expense, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: SAP Concur Expense
provider_slug: sap-concur-expense
slug: sap-concur-expense-domain-security
source_filename: sap-concur-expense-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.concur.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: false\n- host: developer.concur.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: false\n- host: us.api.concursolutions.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: concur.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: concursolutions.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-concur-expense/refs/heads/main/security/sap-concur-expense-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Expense Management
- Financial Management
- Receipts
- Reimbursement
- Reporting
- SAP
- Travel
---
