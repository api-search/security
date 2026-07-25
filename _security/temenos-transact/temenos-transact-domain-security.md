---
api_specs:
- filename: temenos-transact-accounts-api-openapi.yml
  format: yaml
  label: Temenos Transact Accounts API
  slug: temenos-transact-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/openapi/temenos-transact-accounts-api-openapi.yml
- filename: temenos-transact-beneficiaries-api-openapi.yml
  format: yaml
  label: Temenos Transact Beneficiaries API
  slug: temenos-transact-beneficiaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/openapi/temenos-transact-beneficiaries-api-openapi.yml
- filename: temenos-transact-cards-api-openapi.yml
  format: yaml
  label: Temenos Transact Cards API
  slug: temenos-transact-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/openapi/temenos-transact-cards-api-openapi.yml
- filename: temenos-transact-customers-api-openapi.yml
  format: yaml
  label: Temenos Transact Customers API
  slug: temenos-transact-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/openapi/temenos-transact-customers-api-openapi.yml
- filename: temenos-transact-deposits-api-openapi.yml
  format: yaml
  label: Temenos Transact Deposits API
  slug: temenos-transact-deposits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/openapi/temenos-transact-deposits-api-openapi.yml
- filename: temenos-transact-loans-api-openapi.yml
  format: yaml
  label: Temenos Transact Loans API
  slug: temenos-transact-loans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/openapi/temenos-transact-loans-api-openapi.yml
- filename: temenos-transact-payments-api-openapi.yml
  format: yaml
  label: Temenos Transact Payments API
  slug: temenos-transact-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/openapi/temenos-transact-payments-api-openapi.yml
- filename: temenos-transact-products-api-openapi.yml
  format: yaml
  label: Temenos Transact Products API
  slug: temenos-transact-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/openapi/temenos-transact-products-api-openapi.yml
- filename: temenos-transact-reference-data-api-openapi.yml
  format: yaml
  label: Temenos Transact Reference Data API
  slug: temenos-transact-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/openapi/temenos-transact-reference-data-api-openapi.yml
- filename: temenos-transact-transactions-api-openapi.yml
  format: yaml
  label: Temenos Transact Transactions API
  slug: temenos-transact-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/openapi/temenos-transact-transactions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: temenos.com
  spf: true
hosts:
- cert_expires: Sep 30 20:13:58 2026 GMT
  host: developer.temenos.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 30 20:13:58 2026 GMT
  host: www.temenos.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Jul 14 23:59:59 2026 GMT
  host: api.temenos.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Temenos Transact Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Temenos Transact, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Temenos Transact
provider_slug: temenos-transact
slug: temenos-transact-domain-security
source_filename: temenos-transact-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.temenos.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 30 20:13:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.temenos.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 30 20:13:58 2026 GMT\n  hsts: false\n- host: api.temenos.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jul 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: temenos.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/security/temenos-transact-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Banking
- Core Banking
- Digital Banking
- Enterprise
- Financial Services
- Fintech
---
