---
api_specs:
- filename: wingspan-1099-operations-api-openapi.yml
  format: yaml
  label: Wingspan 1099 Operations API
  slug: wingspan-1099-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wingspan/refs/heads/main/openapi/wingspan-1099-operations-api-openapi.yml
- filename: wingspan-banking-management-api-openapi.yml
  format: yaml
  label: Wingspan Banking Management API
  slug: wingspan-banking-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wingspan/refs/heads/main/openapi/wingspan-banking-management-api-openapi.yml
- filename: wingspan-bulk-operations-api-openapi.yml
  format: yaml
  label: Wingspan Bulk Operations API
  slug: wingspan-bulk-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wingspan/refs/heads/main/openapi/wingspan-bulk-operations-api-openapi.yml
- filename: wingspan-client-management-api-openapi.yml
  format: yaml
  label: Wingspan Client Management API
  slug: wingspan-client-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wingspan/refs/heads/main/openapi/wingspan-client-management-api-openapi.yml
- filename: wingspan-collaborator-management-api-openapi.yml
  format: yaml
  label: Wingspan Collaborator Management API
  slug: wingspan-collaborator-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wingspan/refs/heads/main/openapi/wingspan-collaborator-management-api-openapi.yml
- filename: wingspan-custom-field-management-api-openapi.yml
  format: yaml
  label: Wingspan Custom Field Management API
  slug: wingspan-custom-field-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wingspan/refs/heads/main/openapi/wingspan-custom-field-management-api-openapi.yml
- filename: wingspan-deprecated-api-openapi.yml
  format: yaml
  label: Wingspan Deprecated API
  slug: wingspan-deprecated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wingspan/refs/heads/main/openapi/wingspan-deprecated-api-openapi.yml
- filename: wingspan-document-signing-and-eligibility-api-openapi.yml
  format: yaml
  label: Wingspan Document Signing and Eligibility API
  slug: wingspan-document-signing-and-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wingspan/refs/heads/main/openapi/wingspan-document-signing-and-eligibility-api-openapi.yml
- filename: wingspan-invoice-management-api-openapi.yml
  format: yaml
  label: Wingspan Invoice Management API
  slug: wingspan-invoice-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wingspan/refs/heads/main/openapi/wingspan-invoice-management-api-openapi.yml
- filename: wingspan-merchant-category-codes-api-openapi.yml
  format: yaml
  label: Wingspan Merchant Category Codes API
  slug: wingspan-merchant-category-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wingspan/refs/heads/main/openapi/wingspan-merchant-category-codes-api-openapi.yml
- filename: wingspan-payables-management-api-openapi.yml
  format: yaml
  label: Wingspan Payables Management API
  slug: wingspan-payables-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wingspan/refs/heads/main/openapi/wingspan-payables-management-api-openapi.yml
- filename: wingspan-payroll-settings-api-openapi.yml
  format: yaml
  label: Wingspan Payroll Settings API
  slug: wingspan-payroll-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wingspan/refs/heads/main/openapi/wingspan-payroll-settings-api-openapi.yml
- filename: wingspan-reporting-and-analytics-api-openapi.yml
  format: yaml
  label: Wingspan Reporting and Analytics API
  slug: wingspan-reporting-and-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wingspan/refs/heads/main/openapi/wingspan-reporting-and-analytics-api-openapi.yml
- filename: wingspan-service-settings-api-openapi.yml
  format: yaml
  label: Wingspan Service Settings API
  slug: wingspan-service-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wingspan/refs/heads/main/openapi/wingspan-service-settings-api-openapi.yml
- filename: wingspan-wingspan-wallet-api-openapi.yml
  format: yaml
  label: Wingspan Wingspan Wallet API
  slug: wingspan-wingspan-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wingspan/refs/heads/main/openapi/wingspan-wingspan-wallet-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wingspan.app
  spf: true
hosts:
- cert_expires: Oct  5 12:24:59 2026 GMT
  host: api.wingspan.app
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 09:47:55 2026 GMT
  host: stagingapi.wingspan.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wingspan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wingspan, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Wingspan
provider_slug: wingspan
slug: wingspan-domain-security
source_filename: wingspan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.wingspan.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 12:24:59 2026 GMT\n  hsts: null\n- host: stagingapi.wingspan.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 09:47:55 2026 GMT\n  hsts: null\ndomains:\n- domain: wingspan.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wingspan/refs/heads/main/security/wingspan-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Payments
- Payroll
- Contractors
- Invoicing
- Taxes
- Fintech
- Freelance Economy
---
