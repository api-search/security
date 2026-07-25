---
api_specs:
- filename: oracle-financials-budgetary-control-api-openapi.yml
  format: yaml
  label: Oracle Financials Budgetary Control API
  slug: oracle-financials-budgetary-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-financials/refs/heads/main/openapi/oracle-financials-budgetary-control-api-openapi.yml
- filename: oracle-financials-chart-of-accounts-api-openapi.yml
  format: yaml
  label: Oracle Financials Chart of Accounts API
  slug: oracle-financials-chart-of-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-financials/refs/heads/main/openapi/oracle-financials-chart-of-accounts-api-openapi.yml
- filename: oracle-financials-currency-rates-api-openapi.yml
  format: yaml
  label: Oracle Financials Currency Rates API
  slug: oracle-financials-currency-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-financials/refs/heads/main/openapi/oracle-financials-currency-rates-api-openapi.yml
- filename: oracle-financials-journal-batches-api-openapi.yml
  format: yaml
  label: Oracle Financials Journal Batches API
  slug: oracle-financials-journal-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-financials/refs/heads/main/openapi/oracle-financials-journal-batches-api-openapi.yml
- filename: oracle-financials-ledger-balances-api-openapi.yml
  format: yaml
  label: Oracle Financials Ledger Balances API
  slug: oracle-financials-ledger-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-financials/refs/heads/main/openapi/oracle-financials-ledger-balances-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: oracle.com
  spf: true
- caa:
  - 0 issue "symantec.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: oraclecloud.com
  spf: true
hosts:
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: docs.oracle.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 23:59:59 2026 GMT
  host: your-instance.fa.us2.oraclecloud.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oracle Financials Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oracle Financials, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Oracle Financials
provider_slug: oracle-financials
slug: oracle-financials-domain-security
source_filename: oracle-financials-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.oracle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: false\n- host: your-instance.fa.us2.oraclecloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: oracle.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: oraclecloud.com\n  dnssec: false\n  caa:\n  - 0 issue \"symantec.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-financials/refs/heads/main/security/oracle-financials-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Accounting
- Accounts Payable
- Accounts Receivable
- Cash Management
- ERP
- Expense Management
- Financial Management
- General Ledger
---
