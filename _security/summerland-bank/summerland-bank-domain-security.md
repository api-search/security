---
api_specs:
- filename: summerland-bank-banking-account-balances-api-openapi.yml
  format: yaml
  label: Summerland Bank Banking Account Balances API
  slug: summerland-bank-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/summerland-bank/refs/heads/main/openapi/summerland-bank-banking-account-balances-api-openapi.yml
- filename: summerland-bank-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: Summerland Bank Banking Account Direct Debits API
  slug: summerland-bank-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/summerland-bank/refs/heads/main/openapi/summerland-bank-banking-account-direct-debits-api-openapi.yml
- filename: summerland-bank-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: Summerland Bank Banking Account Scheduled Payments API
  slug: summerland-bank-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/summerland-bank/refs/heads/main/openapi/summerland-bank-banking-account-scheduled-payments-api-openapi.yml
- filename: summerland-bank-banking-account-transactions-api-openapi.yml
  format: yaml
  label: Summerland Bank Banking Account Transactions API
  slug: summerland-bank-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/summerland-bank/refs/heads/main/openapi/summerland-bank-banking-account-transactions-api-openapi.yml
- filename: summerland-bank-banking-accounts-api-openapi.yml
  format: yaml
  label: Summerland Bank Banking Accounts API
  slug: summerland-bank-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/summerland-bank/refs/heads/main/openapi/summerland-bank-banking-accounts-api-openapi.yml
- filename: summerland-bank-banking-payees-api-openapi.yml
  format: yaml
  label: Summerland Bank Banking Payees API
  slug: summerland-bank-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/summerland-bank/refs/heads/main/openapi/summerland-bank-banking-payees-api-openapi.yml
- filename: summerland-bank-banking-products-api-openapi.yml
  format: yaml
  label: Summerland Bank Banking Products API
  slug: summerland-bank-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/summerland-bank/refs/heads/main/openapi/summerland-bank-banking-products-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "digicert.com"
  - 0 issuewild "amazon.com"
  - 0 iodef "mailto:it@summerland.com.au"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: summerland.com.au
  spf: true
hosts:
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: www.summerland.com.au
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 19:34:34 2026 GMT
  host: public.cdr-api.summerland.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Summerland Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Summerland Bank, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Summerland Bank
provider_slug: summerland-bank
slug: summerland-bank-domain-security
source_filename: summerland-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.summerland.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: public.cdr-api.summerland.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 19:34:34 2026 GMT\n  hsts: null\ndomains:\n- domain: summerland.com.au\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 iodef \"mailto:it@summerland.com.au\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/summerland-bank/refs/heads/main/security/summerland-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Data Right
- Consumer Banking
- Australia
- Mutual Bank
---
