---
api_specs:
- filename: plansource-aca-api-openapi.yml
  format: yaml
  label: PlanSource ACA API
  slug: plansource-aca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plansource/refs/heads/main/openapi/plansource-aca-api-openapi.yml
- filename: plansource-administrators-api-openapi.yml
  format: yaml
  label: PlanSource Administrators API
  slug: plansource-administrators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plansource/refs/heads/main/openapi/plansource-administrators-api-openapi.yml
- filename: plansource-collections-api-openapi.yml
  format: yaml
  label: PlanSource Collections API
  slug: plansource-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plansource/refs/heads/main/openapi/plansource-collections-api-openapi.yml
- filename: plansource-coverage-api-openapi.yml
  format: yaml
  label: PlanSource Coverage API
  slug: plansource-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plansource/refs/heads/main/openapi/plansource-coverage-api-openapi.yml
- filename: plansource-demographic-api-openapi.yml
  format: yaml
  label: PlanSource Demographic API
  slug: plansource-demographic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plansource/refs/heads/main/openapi/plansource-demographic-api-openapi.yml
- filename: plansource-eoi-api-openapi.yml
  format: yaml
  label: PlanSource EOI API
  slug: plansource-eoi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plansource/refs/heads/main/openapi/plansource-eoi-api-openapi.yml
- filename: plansource-page-content-api-openapi.yml
  format: yaml
  label: PlanSource Page Content API
  slug: plansource-page-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plansource/refs/heads/main/openapi/plansource-page-content-api-openapi.yml
- filename: plansource-payroll-api-openapi.yml
  format: yaml
  label: PlanSource Payroll API
  slug: plansource-payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plansource/refs/heads/main/openapi/plansource-payroll-api-openapi.yml
- filename: plansource-security-api-openapi.yml
  format: yaml
  label: PlanSource Security API
  slug: plansource-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plansource/refs/heads/main/openapi/plansource-security-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: plansource.com
  spf: true
hosts:
- cert_expires: Oct  7 13:46:07 2026 GMT
  host: plansource.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 04:38:22 2026 GMT
  host: developer.plansource.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 14:40:48 2027 GMT
  host: api.plansource.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Plansource Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PlanSource, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PlanSource
provider_slug: plansource
slug: plansource-domain-security
source_filename: plansource-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: plansource.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 13:46:07 2026 GMT\n  hsts: false\n- host: developer.plansource.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 04:38:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.plansource.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 20 14:40:48 2027 GMT\n  hsts: null\ndomains:\n- domain: plansource.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plansource/refs/heads/main/security/plansource-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Employee Benefits
- Benefits Administration
- Insurance
- Human Resources
- Payroll
- Health Insurance
- Enrollment
- HR Technology
- Evidence of Insurability
- ACA Reporting
- Eligibility
- Single Sign-On
---
