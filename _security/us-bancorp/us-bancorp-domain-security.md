---
api_specs:
- filename: us-bancorp-accounts-api-openapi.yml
  format: yaml
  label: US Bancorp Accounts API
  slug: us-bancorp-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-bancorp/refs/heads/main/openapi/us-bancorp-accounts-api-openapi.yml
- filename: us-bancorp-balances-api-openapi.yml
  format: yaml
  label: US Bancorp Balances API
  slug: us-bancorp-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-bancorp/refs/heads/main/openapi/us-bancorp-balances-api-openapi.yml
- filename: us-bancorp-credit-transfers-api-openapi.yml
  format: yaml
  label: US Bancorp Credit Transfers API
  slug: us-bancorp-credit-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-bancorp/refs/heads/main/openapi/us-bancorp-credit-transfers-api-openapi.yml
- filename: us-bancorp-exception-history-api-openapi.yml
  format: yaml
  label: US Bancorp Exception History API
  slug: us-bancorp-exception-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-bancorp/refs/heads/main/openapi/us-bancorp-exception-history-api-openapi.yml
- filename: us-bancorp-exceptions-api-openapi.yml
  format: yaml
  label: US Bancorp Exceptions API
  slug: us-bancorp-exceptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-bancorp/refs/heads/main/openapi/us-bancorp-exceptions-api-openapi.yml
- filename: us-bancorp-push-to-card-payments-api-openapi.yml
  format: yaml
  label: US Bancorp Push to Card Payments API
  slug: us-bancorp-push-to-card-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-bancorp/refs/heads/main/openapi/us-bancorp-push-to-card-payments-api-openapi.yml
- filename: us-bancorp-request-for-payment-api-openapi.yml
  format: yaml
  label: US Bancorp Request for Payment API
  slug: us-bancorp-request-for-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-bancorp/refs/heads/main/openapi/us-bancorp-request-for-payment-api-openapi.yml
- filename: us-bancorp-rtp-eligibility-api-openapi.yml
  format: yaml
  label: US Bancorp RTP Eligibility API
  slug: us-bancorp-rtp-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-bancorp/refs/heads/main/openapi/us-bancorp-rtp-eligibility-api-openapi.yml
- filename: us-bancorp-transactions-api-openapi.yml
  format: yaml
  label: US Bancorp Transactions API
  slug: us-bancorp-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-bancorp/refs/heads/main/openapi/us-bancorp-transactions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:domainadmin@usbank.com"
  - 0 iodef "mailto:certificateservicesshared@usbank.com"
  - 0 issue "digicert.com"
  - 0 issue "entrust.net"
  - 0 issuewild ";"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: usbank.com
  spf: true
hosts:
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: developer.usbank.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 12 23:59:59 2027 GMT
  host: api.usbank.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Us Bancorp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for US Bancorp, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: US Bancorp
provider_slug: us-bancorp
slug: us-bancorp-domain-security
source_filename: us-bancorp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.usbank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.usbank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 12 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: usbank.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:domainadmin@usbank.com\"\n  - 0 iodef \"mailto:certificateservicesshared@usbank.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issuewild \";\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-bancorp/refs/heads/main/security/us-bancorp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Banking
- Finance
- Fortune 500
- Corporate Banking
- Payments
- Open Banking
- Treasury Management
- Consumer Banking
---
