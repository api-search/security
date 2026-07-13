---
api_specs:
- filename: Financial_Management.json
  format: json
  label: Workday Financial Management API
  slug: workday-financial-management-api
  spec_type: OpenAPI
  url: https://community.workday.com/sites/default/files/file-hosting/productionapi/Financial_Management/v38.2/Financial_Management.json
- filename: Revenue_Management.json
  format: json
  label: Workday Revenue Management API
  slug: workday-revenue-management-api
  spec_type: OpenAPI
  url: https://community.workday.com/sites/default/files/file-hosting/productionapi/Revenue_Management/v38.2/Revenue_Management.json
- filename: Expenses.json
  format: json
  label: Workday Expenses API
  slug: workday-expenses-api
  spec_type: OpenAPI
  url: https://community.workday.com/sites/default/files/file-hosting/productionapi/Expenses/v38.2/Expenses.json
- filename: Resource_Management.json
  format: json
  label: Workday Procurement API
  slug: workday-procurement-api
  spec_type: OpenAPI
  url: https://community.workday.com/sites/default/files/file-hosting/productionapi/Resource_Management/v38.2/Resource_Management.json
- filename: Cash_Management.json
  format: json
  label: Workday Cash Management API
  slug: workday-cash-management-api
  spec_type: OpenAPI
  url: https://community.workday.com/sites/default/files/file-hosting/productionapi/Cash_Management/v38.2/Cash_Management.json
- filename: Financial_Management.json
  format: json
  label: Workday Financial Accounting API
  slug: workday-financial-accounting-api
  spec_type: OpenAPI
  url: https://community.workday.com/sites/default/files/file-hosting/productionapi/Financial_Management/v38.2/Financial_Management.json
- filename: Report_as_a_Service.json
  format: json
  label: Workday Reporting API
  slug: workday-reporting-api
  spec_type: OpenAPI
  url: https://community.workday.com/sites/default/files/file-hosting/productionapi/Report_as_a_Service/v38.2/Report_as_a_Service.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: workday.com
  spf: true
hosts:
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: www.workday.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 03:09:01 2026 GMT
  host: api.workday.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Workday Financials Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Workday Financials, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Workday Financials
provider_slug: workday-financials
slug: workday-financials-domain-security
source_filename: workday-financials-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.workday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.workday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 03:09:01 2026 GMT\n  hsts: null\ndomains:\n- domain: workday.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-financials/refs/heads/main/security/workday-financials-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Accounting
- Cloud ERP
- Financial Management
- Procurement
---
