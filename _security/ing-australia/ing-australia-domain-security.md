---
api_specs:
- filename: ing-australia-cds-banking-products-openapi.yml
  format: yaml
  label: ING Australia CDR Product Reference Data API
  slug: ing-australia-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ing-australia/refs/heads/main/openapi/ing-australia-cds-banking-products-openapi.yml
- filename: ing-australia-cds-banking-products-openapi.yml
  format: yaml
  label: ING Australia CDR Accounts & Balances API
  slug: ing-australia-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ing-australia/refs/heads/main/openapi/ing-australia-cds-banking-products-openapi.yml
- filename: ing-australia-cds-banking-products-openapi.yml
  format: yaml
  label: ING Australia CDR Transactions API
  slug: ing-australia-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ing-australia/refs/heads/main/openapi/ing-australia-cds-banking-products-openapi.yml
- filename: ing-australia-cds-banking-products-openapi.yml
  format: yaml
  label: ING Australia CDR Direct Debits & Scheduled Payments API
  slug: ing-australia-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ing-australia/refs/heads/main/openapi/ing-australia-cds-banking-products-openapi.yml
- filename: ing-australia-cds-banking-products-openapi.yml
  format: yaml
  label: ING Australia CDR Payees API
  slug: ing-australia-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ing-australia/refs/heads/main/openapi/ing-australia-cds-banking-products-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "identrust.com"
  - 0 issuewild "identrust.com"
  - 0 iodef "mailto:ing.certificate.management@ing.com"
  - 0 issue "swisssign.com"
  - 0 issuewild "entrust.net"
  - 0 issuewild "swisssign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ing.com.au
  spf: true
hosts:
- cert_expires: Oct  8 03:06:20 2026 GMT
  host: www.ing.com.au
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 04:25:38 2026 GMT
  host: id.ob.ing.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ing Australia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ING Australia, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ING Australia
provider_slug: ing-australia
slug: ing-australia-domain-security
source_filename: ing-australia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ing.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 03:06:20 2026 GMT\n  hsts: true\n  hsts_max_age: 16070400\n- host: id.ob.ing.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 04:25:38 2026 GMT\n  hsts: null\ndomains:\n- domain: ing.com.au\n  dnssec: false\n  caa:\n  - 0 issue \"identrust.com\"\n  - 0 issuewild \"identrust.com\"\n  - 0 iodef \"mailto:ing.certificate.management@ing.com\"\n  - 0 issue \"swisssign.com\"\n  - 0 issuewild \"entrust.net\"\n  - 0 issuewild \"swisssign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ing-australia/refs/heads/main/security/ing-australia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Product Reference Data
- ADI
---
