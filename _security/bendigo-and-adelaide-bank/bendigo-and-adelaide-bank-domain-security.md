---
api_specs:
- filename: bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Bendigo and Adelaide Bank CDR Product Reference Data API
  slug: bendigo-and-adelaide-bank-cds-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bendigo-and-adelaide-bank/refs/heads/main/openapi/bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
- filename: bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Bendigo and Adelaide Bank CDR Accounts & Balances API
  slug: bendigo-and-adelaide-bank-cds-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bendigo-and-adelaide-bank/refs/heads/main/openapi/bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
- filename: bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Bendigo and Adelaide Bank CDR Transactions API
  slug: bendigo-and-adelaide-bank-cds-banking-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bendigo-and-adelaide-bank/refs/heads/main/openapi/bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
- filename: bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Bendigo and Adelaide Bank CDR Direct Debits & Scheduled Payments API
  slug: bendigo-and-adelaide-bank-cds-banking-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bendigo-and-adelaide-bank/refs/heads/main/openapi/bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
- filename: bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Bendigo and Adelaide Bank CDR Payees API
  slug: bendigo-and-adelaide-bank-cds-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bendigo-and-adelaide-bank/refs/heads/main/openapi/bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
- filename: bendigo-and-adelaide-bank-up-developer-api-openapi.json
  format: json
  label: Up Developer API (Personal Banking)
  slug: up-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bendigo-and-adelaide-bank/refs/heads/main/openapi/bendigo-and-adelaide-bank-up-developer-api-openapi.json
- filename: bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Up Banking CDR Product Reference Data API
  slug: up-cds-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bendigo-and-adelaide-bank/refs/heads/main/openapi/bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
- filename: bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Adelaide Bank CDR Product Reference Data API
  slug: adelaide-bank-cds-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bendigo-and-adelaide-bank/refs/heads/main/openapi/bendigo-and-adelaide-bank-cds-banking-products-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "entrust.net"
  - 0 iodef "mailto:DomainAlerts@bendigobank.com.au"
  - 0 issue "ssl.com"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bendigobank.com.au
  spf: true
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 iodef "mailto:DomainAlerts@bendigobank.com.au"
  - 0 issue "entrust.net"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bendigoadelaide.com.au
  spf: true
hosts:
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: www.bendigobank.com.au
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 23:59:59 2026 GMT
  host: www.bendigoadelaide.com.au
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: api.cdr.bendigobank.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bendigo And Adelaide Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bendigo and Adelaide Bank, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bendigo and Adelaide Bank
provider_slug: bendigo-and-adelaide-bank
slug: bendigo-and-adelaide-bank-domain-security
source_filename: bendigo-and-adelaide-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bendigobank.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: www.bendigoadelaide.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: api.cdr.bendigobank.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: bendigobank.com.au\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"entrust.net\"\n  - 0 iodef \"mailto:DomainAlerts@bendigobank.com.au\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: bendigoadelaide.com.au\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 iodef \"mailto:DomainAlerts@bendigobank.com.au\"\
  \n  - 0 issue \"entrust.net\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bendigo-and-adelaide-bank/refs/heads/main/security/bendigo-and-adelaide-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Data Right
- Consumer Banking
- Australia
- Product Reference Data
---
