---
api_specs:
- filename: oracle-general-ledger-accounting-periods-api-openapi.yml
  format: yaml
  label: Oracle General Ledger Accounting Periods API
  slug: oracle-general-ledger-accounting-periods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-general-ledger/refs/heads/main/openapi/oracle-general-ledger-accounting-periods-api-openapi.yml
- filename: oracle-general-ledger-budgetary-control-api-openapi.yml
  format: yaml
  label: Oracle General Ledger Budgetary Control API
  slug: oracle-general-ledger-budgetary-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-general-ledger/refs/heads/main/openapi/oracle-general-ledger-budgetary-control-api-openapi.yml
- filename: oracle-general-ledger-currency-rates-api-openapi.yml
  format: yaml
  label: Oracle General Ledger Currency Rates API
  slug: oracle-general-ledger-currency-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-general-ledger/refs/heads/main/openapi/oracle-general-ledger-currency-rates-api-openapi.yml
- filename: oracle-general-ledger-erp-integrations-api-openapi.yml
  format: yaml
  label: Oracle General Ledger ERP Integrations API
  slug: oracle-general-ledger-erp-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-general-ledger/refs/heads/main/openapi/oracle-general-ledger-erp-integrations-api-openapi.yml
- filename: oracle-general-ledger-intercompany-api-openapi.yml
  format: yaml
  label: Oracle General Ledger Intercompany API
  slug: oracle-general-ledger-intercompany-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-general-ledger/refs/heads/main/openapi/oracle-general-ledger-intercompany-api-openapi.yml
- filename: oracle-general-ledger-journal-batches-api-openapi.yml
  format: yaml
  label: Oracle General Ledger Journal Batches API
  slug: oracle-general-ledger-journal-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-general-ledger/refs/heads/main/openapi/oracle-general-ledger-journal-batches-api-openapi.yml
- filename: oracle-general-ledger-ledger-balances-api-openapi.yml
  format: yaml
  label: Oracle General Ledger Ledger Balances API
  slug: oracle-general-ledger-ledger-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-general-ledger/refs/heads/main/openapi/oracle-general-ledger-ledger-balances-api-openapi.yml
- filename: oracle-general-ledger-ledger-options-api-openapi.yml
  format: yaml
  label: Oracle General Ledger Ledger Options API
  slug: oracle-general-ledger-ledger-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-general-ledger/refs/heads/main/openapi/oracle-general-ledger-ledger-options-api-openapi.yml
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
hosts:
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: docs.oracle.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  7 23:59:59 2027 GMT
  host: www.oracle.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oracle General Ledger Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oracle General Ledger, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Oracle General Ledger
provider_slug: oracle-general-ledger
slug: oracle-general-ledger-domain-security
source_filename: oracle-general-ledger-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.oracle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: false\n- host: www.oracle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: oracle.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-general-ledger/refs/heads/main/security/oracle-general-ledger-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Accounting
- Balances
- Cloud
- ERP
- Finance
- General Ledger
- Journals
---
