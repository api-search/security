---
api_specs:
- filename: bankday-dev-account-api-openapi.yml
  format: yaml
  label: bankday-dev Account API
  slug: bankday-dev-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bankday-dev/openapi/bankday-dev-account-api-openapi.yml
- filename: bankday-dev-ach-api-openapi.yml
  format: yaml
  label: bankday-dev Ach API
  slug: bankday-dev-ach-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bankday-dev/openapi/bankday-dev-ach-api-openapi.yml
- filename: bankday-dev-business-day-api-openapi.yml
  format: yaml
  label: bankday-dev Business Day API
  slug: bankday-dev-business-day-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bankday-dev/openapi/bankday-dev-business-day-api-openapi.yml
- filename: bankday-dev-business-days-api-openapi.yml
  format: yaml
  label: bankday-dev Business Days API
  slug: bankday-dev-business-days-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bankday-dev/openapi/bankday-dev-business-days-api-openapi.yml
- filename: bankday-dev-calendars-api-openapi.yml
  format: yaml
  label: bankday-dev Calendars API
  slug: bankday-dev-calendars-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bankday-dev/openapi/bankday-dev-calendars-api-openapi.yml
- filename: bankday-dev-fx-api-openapi.yml
  format: yaml
  label: bankday-dev Fx API
  slug: bankday-dev-fx-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bankday-dev/openapi/bankday-dev-fx-api-openapi.yml
- filename: bankday-dev-holidays-api-openapi.yml
  format: yaml
  label: bankday-dev Holidays API
  slug: bankday-dev-holidays-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bankday-dev/openapi/bankday-dev-holidays-api-openapi.yml
- filename: bankday-dev-minimum-wage-api-openapi.yml
  format: yaml
  label: bankday-dev Minimum Wage API
  slug: bankday-dev-minimum-wage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bankday-dev/openapi/bankday-dev-minimum-wage-api-openapi.yml
- filename: bankday-dev-payroll-api-openapi.yml
  format: yaml
  label: bankday-dev Payroll API
  slug: bankday-dev-payroll-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bankday-dev/openapi/bankday-dev-payroll-api-openapi.yml
- filename: bankday-dev-today-api-openapi.yml
  format: yaml
  label: bankday-dev Today API
  slug: bankday-dev-today-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bankday-dev/openapi/bankday-dev-today-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bankday.dev
  spf: true
hosts:
- cert_expires: Jan 14 21:43:59 2027 GMT
  host: bankday.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bankday Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for bankday-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: bankday-dev
provider_slug: bankday-dev
slug: bankday-dev-domain-security
source_filename: bankday-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bankday.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 21:43:59 2027 GMT\n  hsts: false\ndomains:\n- domain: bankday.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/bankday-dev/security/bankday-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Finance
- Calendar
- API
- Payments
---
