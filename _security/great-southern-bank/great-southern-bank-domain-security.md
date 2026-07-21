---
api_specs:
- filename: great-southern-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Great Southern Bank CDR Product Reference Data API
  slug: great-southern-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/great-southern-bank/refs/heads/main/openapi/great-southern-bank-cds-banking-products-openapi.yml
- filename: great-southern-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Great Southern Bank Business+ CDR Product Reference Data API
  slug: great-southern-bank-business-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/great-southern-bank/refs/heads/main/openapi/great-southern-bank-cds-banking-products-openapi.yml
- filename: great-southern-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Great Southern Bank CDR Accounts & Balances API
  slug: great-southern-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/great-southern-bank/refs/heads/main/openapi/great-southern-bank-cds-banking-products-openapi.yml
- filename: great-southern-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Great Southern Bank CDR Transactions API
  slug: great-southern-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/great-southern-bank/refs/heads/main/openapi/great-southern-bank-cds-banking-products-openapi.yml
- filename: great-southern-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Great Southern Bank CDR Direct Debits & Scheduled Payments API
  slug: great-southern-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/great-southern-bank/refs/heads/main/openapi/great-southern-bank-cds-banking-products-openapi.yml
- filename: great-southern-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Great Southern Bank CDR Payees API
  slug: great-southern-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/great-southern-bank/refs/heads/main/openapi/great-southern-bank-cds-banking-products-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild ";"
  - 0 iodef "mailto:dns.admin@gsb.com.au"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: greatsouthernbank.com.au
  spf: true
hosts:
- cert_expires: Aug 31 19:36:02 2026 GMT
  host: www.greatsouthernbank.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 10 23:59:59 2026 GMT
  host: api.open-banking.greatsouthernbank.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: od1.open-banking.business.greatsouthernbank.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Great Southern Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Great Southern Bank, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Great Southern Bank
provider_slug: great-southern-bank
slug: great-southern-bank-domain-security
source_filename: great-southern-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.greatsouthernbank.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 19:36:02 2026 GMT\n  hsts: null\n- host: api.open-banking.greatsouthernbank.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 23:59:59 2026 GMT\n  hsts: null\n- host: od1.open-banking.business.greatsouthernbank.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: greatsouthernbank.com.au\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \";\"\n  - 0 iodef \"mailto:dns.admin@gsb.com.au\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/great-southern-bank/refs/heads/main/security/great-southern-bank-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Customer Owned
- Product Reference Data
---
