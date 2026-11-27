---
api_specs:
- filename: anytax-country-api-api-openapi.yml
  format: yaml
  label: AnyTax Country API
  slug: anytax-country-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anytax/openapi/anytax-country-api-api-openapi.yml
- filename: anytax-e-r-api-api-openapi.yml
  format: yaml
  label: AnyTax EÜR API
  slug: anytax-e-r-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anytax/openapi/anytax-e-r-api-api-openapi.yml
- filename: anytax-elster-import-api-api-openapi.yml
  format: yaml
  label: AnyTax ELSTER Import API
  slug: anytax-elster-import-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anytax/openapi/anytax-elster-import-api-api-openapi.yml
- filename: anytax-estimator-api-openapi.yml
  format: yaml
  label: AnyTax Estimator API
  slug: anytax-estimator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anytax/openapi/anytax-estimator-api-openapi.yml
- filename: anytax-filing-api-api-openapi.yml
  format: yaml
  label: AnyTax Filing API
  slug: anytax-filing-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anytax/openapi/anytax-filing-api-api-openapi.yml
- filename: anytax-filing-eligibility-check-api-openapi.yml
  format: yaml
  label: AnyTax Filing Eligibility Check API
  slug: anytax-filing-eligibility-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anytax/openapi/anytax-filing-eligibility-check-api-openapi.yml
- filename: anytax-navigation-api-api-openapi.yml
  format: yaml
  label: AnyTax Navigation API
  slug: anytax-navigation-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anytax/openapi/anytax-navigation-api-api-openapi.yml
- filename: anytax-partner-platform-api-openapi.yml
  format: yaml
  label: AnyTax Partner platform API
  slug: anytax-partner-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anytax/openapi/anytax-partner-platform-api-openapi.yml
- filename: anytax-public-api-api-openapi.yml
  format: yaml
  label: AnyTax Public API
  slug: anytax-public-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anytax/openapi/anytax-public-api-api-openapi.yml
- filename: anytax-question-api-api-openapi.yml
  format: yaml
  label: AnyTax Question API
  slug: anytax-question-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anytax/openapi/anytax-question-api-api-openapi.yml
- filename: anytax-scenario-api-api-openapi.yml
  format: yaml
  label: AnyTax Scenario API
  slug: anytax-scenario-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anytax/openapi/anytax-scenario-api-api-openapi.yml
- filename: anytax-tax-saving-tip-api-api-openapi.yml
  format: yaml
  label: AnyTax Tax Saving Tip API
  slug: anytax-tax-saving-tip-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anytax/openapi/anytax-tax-saving-tip-api-api-openapi.yml
- filename: anytax-user-api-api-openapi.yml
  format: yaml
  label: AnyTax User API
  slug: anytax-user-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anytax/openapi/anytax-user-api-api-openapi.yml
- filename: anytax-wage-tax-api-api-openapi.yml
  format: yaml
  label: AnyTax Wage Tax API
  slug: anytax-wage-tax-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anytax/openapi/anytax-wage-tax-api-api-openapi.yml
- filename: anytax-answer-api-api-openapi.yml
  format: yaml
  label: AnyTax Answer API
  slug: anytax-answer-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anytax/openapi/anytax-answer-api-api-openapi.yml
- filename: anytax-auth-api-api-openapi.yml
  format: yaml
  label: AnyTax Auth API
  slug: anytax-auth-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anytax/openapi/anytax-auth-api-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: anytax.io
  spf: true
hosts:
- cert_expires: Jan 12 06:17:26 2027 GMT
  host: anytax.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 00:09:37 2026 GMT
  host: api.anytax.io
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: AnyTax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AnyTax, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AnyTax
provider_slug: anytax
slug: anytax-domain-security
source_filename: anytax-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anytax.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 06:17:26 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.anytax.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 00:09:37 2026 GMT\n  hsts: null\ndomains:\n- domain: anytax.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/anytax/security/anytax-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fintech
- Tax
- Integration
- Banking
- Tax Planning
- White Label
- Compliance
---
