---
api_specs:
- filename: lumabill-ch-account-api-openapi.yml
  format: yaml
  label: LumaBill Account API
  slug: lumabill-ch-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumabill-ch/openapi/lumabill-ch-account-api-openapi.yml
- filename: lumabill-ch-bank-accounts-api-openapi.yml
  format: yaml
  label: LumaBill Bank Accounts API
  slug: lumabill-ch-bank-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumabill-ch/openapi/lumabill-ch-bank-accounts-api-openapi.yml
- filename: lumabill-ch-bank-imports-api-openapi.yml
  format: yaml
  label: LumaBill Bank Imports API
  slug: lumabill-ch-bank-imports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumabill-ch/openapi/lumabill-ch-bank-imports-api-openapi.yml
- filename: lumabill-ch-catalog-api-openapi.yml
  format: yaml
  label: LumaBill Catalog API
  slug: lumabill-ch-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumabill-ch/openapi/lumabill-ch-catalog-api-openapi.yml
- filename: lumabill-ch-chart-of-accounts-api-openapi.yml
  format: yaml
  label: LumaBill Chart of Accounts API
  slug: lumabill-ch-chart-of-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumabill-ch/openapi/lumabill-ch-chart-of-accounts-api-openapi.yml
- filename: lumabill-ch-clients-api-openapi.yml
  format: yaml
  label: LumaBill Clients API
  slug: lumabill-ch-clients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumabill-ch/openapi/lumabill-ch-clients-api-openapi.yml
- filename: lumabill-ch-expenses-api-openapi.yml
  format: yaml
  label: LumaBill Expenses API
  slug: lumabill-ch-expenses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumabill-ch/openapi/lumabill-ch-expenses-api-openapi.yml
- filename: lumabill-ch-fiscal-years-api-openapi.yml
  format: yaml
  label: LumaBill Fiscal Years API
  slug: lumabill-ch-fiscal-years-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumabill-ch/openapi/lumabill-ch-fiscal-years-api-openapi.yml
- filename: lumabill-ch-invoices-api-openapi.yml
  format: yaml
  label: LumaBill Invoices API
  slug: lumabill-ch-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumabill-ch/openapi/lumabill-ch-invoices-api-openapi.yml
- filename: lumabill-ch-journal-entries-api-openapi.yml
  format: yaml
  label: LumaBill Journal Entries API
  slug: lumabill-ch-journal-entries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumabill-ch/openapi/lumabill-ch-journal-entries-api-openapi.yml
- filename: lumabill-ch-offers-api-openapi.yml
  format: yaml
  label: LumaBill Offers API
  slug: lumabill-ch-offers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumabill-ch/openapi/lumabill-ch-offers-api-openapi.yml
- filename: lumabill-ch-payments-api-openapi.yml
  format: yaml
  label: LumaBill Payments API
  slug: lumabill-ch-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumabill-ch/openapi/lumabill-ch-payments-api-openapi.yml
- filename: lumabill-ch-profiles-api-openapi.yml
  format: yaml
  label: LumaBill Profiles API
  slug: lumabill-ch-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumabill-ch/openapi/lumabill-ch-profiles-api-openapi.yml
- filename: lumabill-ch-recurring-invoices-api-openapi.yml
  format: yaml
  label: LumaBill Recurring Invoices API
  slug: lumabill-ch-recurring-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumabill-ch/openapi/lumabill-ch-recurring-invoices-api-openapi.yml
- filename: lumabill-ch-reports-api-openapi.yml
  format: yaml
  label: LumaBill Reports API
  slug: lumabill-ch-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumabill-ch/openapi/lumabill-ch-reports-api-openapi.yml
- filename: lumabill-ch-revenue-api-openapi.yml
  format: yaml
  label: LumaBill Revenue API
  slug: lumabill-ch-revenue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumabill-ch/openapi/lumabill-ch-revenue-api-openapi.yml
- filename: lumabill-ch-vendors-api-openapi.yml
  format: yaml
  label: LumaBill Vendors API
  slug: lumabill-ch-vendors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumabill-ch/openapi/lumabill-ch-vendors-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lumabill.ch
  spf: true
hosts:
- cert_expires: Feb 19 23:59:59 2027 GMT
  host: lumabill.ch
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LumaBill Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LumaBill, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LumaBill
provider_slug: lumabill-ch
slug: lumabill-ch-domain-security
source_filename: lumabill-ch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lumabill.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lumabill.ch\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/lumabill-ch/security/lumabill-ch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Accounting
- Invoicing
- Software-as-a-Service
- Switzerland
- Small Business
---
