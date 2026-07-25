---
api_specs:
- filename: zopa-account-access-api-openapi.yml
  format: yaml
  label: zopa Account Access API
  slug: zopa-account-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/openapi/zopa-account-access-api-openapi.yml
- filename: zopa-accounts-api-openapi.yml
  format: yaml
  label: zopa Accounts API
  slug: zopa-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/openapi/zopa-accounts-api-openapi.yml
- filename: zopa-balances-api-openapi.yml
  format: yaml
  label: zopa Balances API
  slug: zopa-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/openapi/zopa-balances-api-openapi.yml
- filename: zopa-beneficiaries-api-openapi.yml
  format: yaml
  label: zopa Beneficiaries API
  slug: zopa-beneficiaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/openapi/zopa-beneficiaries-api-openapi.yml
- filename: zopa-direct-debits-api-openapi.yml
  format: yaml
  label: zopa Direct Debits API
  slug: zopa-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/openapi/zopa-direct-debits-api-openapi.yml
- filename: zopa-domestic-payments-api-openapi.yml
  format: yaml
  label: zopa Domestic Payments API
  slug: zopa-domestic-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/openapi/zopa-domestic-payments-api-openapi.yml
- filename: zopa-domestic-standing-orders-api-openapi.yml
  format: yaml
  label: zopa Domestic Standing Orders API
  slug: zopa-domestic-standing-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/openapi/zopa-domestic-standing-orders-api-openapi.yml
- filename: zopa-offers-api-openapi.yml
  format: yaml
  label: zopa Offers API
  slug: zopa-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/openapi/zopa-offers-api-openapi.yml
- filename: zopa-parties-api-openapi.yml
  format: yaml
  label: zopa Parties API
  slug: zopa-parties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/openapi/zopa-parties-api-openapi.yml
- filename: zopa-standing-orders-api-openapi.yml
  format: yaml
  label: zopa Standing Orders API
  slug: zopa-standing-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/openapi/zopa-standing-orders-api-openapi.yml
- filename: zopa-statements-api-openapi.yml
  format: yaml
  label: zopa Statements API
  slug: zopa-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/openapi/zopa-statements-api-openapi.yml
- filename: zopa-transactions-api-openapi.yml
  format: yaml
  label: zopa Transactions API
  slug: zopa-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/openapi/zopa-transactions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zopa.com
  spf: true
hosts:
- cert_expires: Sep 27 23:59:59 2026 GMT
  host: www.zopa.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zopa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for zopa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: zopa
provider_slug: zopa
slug: zopa-domain-security
source_filename: zopa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zopa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: zopa.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/security/zopa-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Banking
- Fintech
- Open Banking
- PSD2
- Payments
- Account Information
- Payment Initiation
- FAPI
- United Kingdom
- Digital Bank
- Lending
---
