---
api_specs:
- filename: taxjar-categories-api-openapi.yml
  format: yaml
  label: TaxJar Categories API
  slug: taxjar-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taxjar/refs/heads/main/openapi/taxjar-categories-api-openapi.yml
- filename: taxjar-customers-api-openapi.yml
  format: yaml
  label: TaxJar Customers API
  slug: taxjar-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taxjar/refs/heads/main/openapi/taxjar-customers-api-openapi.yml
- filename: taxjar-nexus-api-openapi.yml
  format: yaml
  label: TaxJar Nexus API
  slug: taxjar-nexus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taxjar/refs/heads/main/openapi/taxjar-nexus-api-openapi.yml
- filename: taxjar-rates-api-openapi.yml
  format: yaml
  label: TaxJar Rates API
  slug: taxjar-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taxjar/refs/heads/main/openapi/taxjar-rates-api-openapi.yml
- filename: taxjar-summary-rates-api-openapi.yml
  format: yaml
  label: TaxJar Summary Rates API
  slug: taxjar-summary-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taxjar/refs/heads/main/openapi/taxjar-summary-rates-api-openapi.yml
- filename: taxjar-taxes-api-openapi.yml
  format: yaml
  label: TaxJar Taxes API
  slug: taxjar-taxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taxjar/refs/heads/main/openapi/taxjar-taxes-api-openapi.yml
- filename: taxjar-transactions-orders-api-openapi.yml
  format: yaml
  label: TaxJar Transactions - Orders API
  slug: taxjar-transactions-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taxjar/refs/heads/main/openapi/taxjar-transactions-orders-api-openapi.yml
- filename: taxjar-transactions-refunds-api-openapi.yml
  format: yaml
  label: TaxJar Transactions - Refunds API
  slug: taxjar-transactions-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taxjar/refs/heads/main/openapi/taxjar-transactions-refunds-api-openapi.yml
- filename: taxjar-validations-api-openapi.yml
  format: yaml
  label: TaxJar Validations API
  slug: taxjar-validations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taxjar/refs/heads/main/openapi/taxjar-validations-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: false
  domain: taxjar.com
  spf: true
hosts:
- cert_expires: Sep  6 23:15:29 2026 GMT
  host: www.taxjar.com
  hsts: true
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 23:15:29 2026 GMT
  host: developers.taxjar.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  2 23:59:59 2027 GMT
  host: api.taxjar.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Taxjar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TaxJar, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present.'
provider_name: TaxJar
provider_slug: taxjar
slug: taxjar-domain-security
source_filename: taxjar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.taxjar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 23:15:29 2026 GMT\n  hsts: true\n- host: developers.taxjar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 23:15:29 2026 GMT\n  hsts: false\n- host: api.taxjar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: taxjar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taxjar/refs/heads/main/security/taxjar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sales Tax
- Tax Compliance
- E-Commerce
- Tax Calculation
- Tax Automation
- Stripe
- FinTech
---
