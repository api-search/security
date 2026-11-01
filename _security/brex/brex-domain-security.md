---
api_specs:
- filename: brex-budget-programs-api-openapi.yml
  format: yaml
  label: Brex Budget Programs API
  slug: brex-budget-programs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brex/openapi/brex-budget-programs-api-openapi.yml
- filename: brex-budgets-api-openapi.yml
  format: yaml
  label: Brex Budgets API
  slug: brex-budgets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brex/openapi/brex-budgets-api-openapi.yml
- filename: brex-spend-limits-api-openapi.yml
  format: yaml
  label: Brex Spend Limits API
  slug: brex-spend-limits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brex/openapi/brex-spend-limits-api-openapi.yml
- filename: brex-cards-api-openapi.yml
  format: yaml
  label: Brex Cards API
  slug: brex-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brex/openapi/brex-cards-api-openapi.yml
- filename: brex-companies-api-openapi.yml
  format: yaml
  label: Brex Companies API
  slug: brex-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brex/openapi/brex-companies-api-openapi.yml
- filename: brex-cost-centers-api-openapi.yml
  format: yaml
  label: Brex Cost Centers API
  slug: brex-cost-centers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brex/openapi/brex-cost-centers-api-openapi.yml
- filename: brex-departments-api-openapi.yml
  format: yaml
  label: Brex Departments API
  slug: brex-departments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brex/openapi/brex-departments-api-openapi.yml
- filename: brex-legal-entities-api-openapi.yml
  format: yaml
  label: Brex Legal Entities API
  slug: brex-legal-entities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brex/openapi/brex-legal-entities-api-openapi.yml
- filename: brex-locations-api-openapi.yml
  format: yaml
  label: Brex Locations API
  slug: brex-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brex/openapi/brex-locations-api-openapi.yml
- filename: brex-titles-api-openapi.yml
  format: yaml
  label: Brex Titles API
  slug: brex-titles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brex/openapi/brex-titles-api-openapi.yml
- filename: brex-users-api-openapi.yml
  format: yaml
  label: Brex Users API
  slug: brex-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brex/openapi/brex-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: brex.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: brexapis.com
  spf: false
hosts:
- cert_expires: Sep 23 17:12:30 2026 GMT
  host: developer.brex.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: platform.brexapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Brex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brex, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Brex
provider_slug: brex
slug: brex-domain-security
source_filename: brex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.brex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 17:12:30 2026 GMT\n  hsts: false\n- host: platform.brexapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: brex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: brexapis.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/brex/security/brex-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Bill Pay
- Corporate Cards
- Expenses
- Reimbursement
- Spending
- Accounting
- Expense Management
---
