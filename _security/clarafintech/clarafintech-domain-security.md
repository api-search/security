---
api_specs:
- filename: clarafintech-accounts-payable-api-openapi.yml
  format: yaml
  label: Clarafintech Accounts Payable API
  slug: clarafintech-accounts-payable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarafintech/refs/heads/main/openapi/clarafintech-accounts-payable-api-openapi.yml
- filename: clarafintech-authentication-api-openapi.yml
  format: yaml
  label: Clarafintech Authentication API
  slug: clarafintech-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarafintech/refs/heads/main/openapi/clarafintech-authentication-api-openapi.yml
- filename: clarafintech-billing-statements-api-openapi.yml
  format: yaml
  label: Clarafintech Billing Statements API
  slug: clarafintech-billing-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarafintech/refs/heads/main/openapi/clarafintech-billing-statements-api-openapi.yml
- filename: clarafintech-cards-api-openapi.yml
  format: yaml
  label: Clarafintech Cards API
  slug: clarafintech-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarafintech/refs/heads/main/openapi/clarafintech-cards-api-openapi.yml
- filename: clarafintech-digital-account-api-openapi.yml
  format: yaml
  label: Clarafintech Digital Account API
  slug: clarafintech-digital-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarafintech/refs/heads/main/openapi/clarafintech-digital-account-api-openapi.yml
- filename: clarafintech-extracted-documents-api-openapi.yml
  format: yaml
  label: Clarafintech Extracted Documents API
  slug: clarafintech-extracted-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarafintech/refs/heads/main/openapi/clarafintech-extracted-documents-api-openapi.yml
- filename: clarafintech-invoices-api-openapi.yml
  format: yaml
  label: Clarafintech Invoices API
  slug: clarafintech-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarafintech/refs/heads/main/openapi/clarafintech-invoices-api-openapi.yml
- filename: clarafintech-reimbursements-api-openapi.yml
  format: yaml
  label: Clarafintech Reimbursements API
  slug: clarafintech-reimbursements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarafintech/refs/heads/main/openapi/clarafintech-reimbursements-api-openapi.yml
- filename: clarafintech-transactions-api-openapi.yml
  format: yaml
  label: Clarafintech Transactions API
  slug: clarafintech-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarafintech/refs/heads/main/openapi/clarafintech-transactions-api-openapi.yml
- filename: clarafintech-users-api-openapi.yml
  format: yaml
  label: Clarafintech Users API
  slug: clarafintech-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarafintech/refs/heads/main/openapi/clarafintech-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: clara.com
  spf: true
hosts:
- cert_expires: Nov 30 18:30:48 2026 GMT
  host: www.clara.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Clarafintech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clarafintech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Clarafintech
provider_slug: clarafintech
slug: clarafintech-domain-security
source_filename: clarafintech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clara.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 18:30:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: clara.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clarafintech/refs/heads/main/security/clarafintech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Fintech
- Spend Management
- Latin America
- Corporate Cards
- Financial Automation
- Company
---
