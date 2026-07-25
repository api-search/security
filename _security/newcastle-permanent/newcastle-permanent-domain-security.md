---
api_specs:
- filename: newcastle-permanent-accounts-api-openapi.yml
  format: yaml
  label: Newcastle Permanent Building Society Accounts API
  slug: newcastle-permanent-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle-permanent/refs/heads/main/openapi/newcastle-permanent-accounts-api-openapi.yml
- filename: newcastle-permanent-banking-account-balances-api-openapi.yml
  format: yaml
  label: Newcastle Permanent Building Society Banking Account Balances API
  slug: newcastle-permanent-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle-permanent/refs/heads/main/openapi/newcastle-permanent-banking-account-balances-api-openapi.yml
- filename: newcastle-permanent-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: Newcastle Permanent Building Society Banking Account Direct Debits API
  slug: newcastle-permanent-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle-permanent/refs/heads/main/openapi/newcastle-permanent-banking-account-direct-debits-api-openapi.yml
- filename: newcastle-permanent-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: Newcastle Permanent Building Society Banking Account Scheduled Payments API
  slug: newcastle-permanent-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle-permanent/refs/heads/main/openapi/newcastle-permanent-banking-account-scheduled-payments-api-openapi.yml
- filename: newcastle-permanent-banking-account-transactions-api-openapi.yml
  format: yaml
  label: Newcastle Permanent Building Society Banking Account Transactions API
  slug: newcastle-permanent-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle-permanent/refs/heads/main/openapi/newcastle-permanent-banking-account-transactions-api-openapi.yml
- filename: newcastle-permanent-banking-accounts-api-openapi.yml
  format: yaml
  label: Newcastle Permanent Building Society Banking Accounts API
  slug: newcastle-permanent-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle-permanent/refs/heads/main/openapi/newcastle-permanent-banking-accounts-api-openapi.yml
- filename: newcastle-permanent-banking-api-openapi.yml
  format: yaml
  label: Newcastle Permanent Building Society Banking API
  slug: newcastle-permanent-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle-permanent/refs/heads/main/openapi/newcastle-permanent-banking-api-openapi.yml
- filename: newcastle-permanent-banking-payees-api-openapi.yml
  format: yaml
  label: Newcastle Permanent Building Society Banking Payees API
  slug: newcastle-permanent-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle-permanent/refs/heads/main/openapi/newcastle-permanent-banking-payees-api-openapi.yml
- filename: newcastle-permanent-banking-products-api-openapi.yml
  format: yaml
  label: Newcastle Permanent Building Society Banking Products API
  slug: newcastle-permanent-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle-permanent/refs/heads/main/openapi/newcastle-permanent-banking-products-api-openapi.yml
- filename: newcastle-permanent-common-api-openapi.yml
  format: yaml
  label: Newcastle Permanent Building Society Common API
  slug: newcastle-permanent-common-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle-permanent/refs/heads/main/openapi/newcastle-permanent-common-api-openapi.yml
- filename: newcastle-permanent-customer-api-openapi.yml
  format: yaml
  label: Newcastle Permanent Building Society Customer API
  slug: newcastle-permanent-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle-permanent/refs/heads/main/openapi/newcastle-permanent-customer-api-openapi.yml
- filename: newcastle-permanent-direct-debits-api-openapi.yml
  format: yaml
  label: Newcastle Permanent Building Society Direct Debits API
  slug: newcastle-permanent-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle-permanent/refs/heads/main/openapi/newcastle-permanent-direct-debits-api-openapi.yml
- filename: newcastle-permanent-payees-api-openapi.yml
  format: yaml
  label: Newcastle Permanent Building Society Payees API
  slug: newcastle-permanent-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle-permanent/refs/heads/main/openapi/newcastle-permanent-payees-api-openapi.yml
- filename: newcastle-permanent-scheduled-payments-api-openapi.yml
  format: yaml
  label: Newcastle Permanent Building Society Scheduled Payments API
  slug: newcastle-permanent-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle-permanent/refs/heads/main/openapi/newcastle-permanent-scheduled-payments-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: newcastlepermanent.com.au
  spf: true
hosts:
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: www.newcastlepermanent.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: developer.newcastlepermanent.com.au
  hsts: true
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep  9 23:59:59 2026 GMT
  host: openbank.newcastlepermanent.com.au
  hsts: true
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Newcastle Permanent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Newcastle Permanent Building Society, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Newcastle Permanent Building Society
provider_slug: newcastle-permanent
slug: newcastle-permanent-domain-security
source_filename: newcastle-permanent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.newcastlepermanent.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: null\n- host: developer.newcastlepermanent.com.au\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: true\n- host: openbank.newcastlepermanent.com.au\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  9 23:59:59 2026 GMT\n  hsts: true\ndomains:\n- domain: newcastlepermanent.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newcastle-permanent/refs/heads/main/security/newcastle-permanent-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Building Society
- Mutual
- Australia
---
