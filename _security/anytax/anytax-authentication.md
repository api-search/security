---
anonymous_access: false
api_key_in:
- header
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
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: AnyTax Authentication
name_suffix: Authentication
oauth_flows: []
overview: AnyTax secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AnyTax
provider_slug: anytax
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearer
  scheme: bearer
  sources:
  - openapi/anytax-openapi.json
  type: http
- description: API key for programmatic authentication
  in: header
  name: api-key
  parameter: X-API-Key
  sources:
  - openapi/anytax-openapi.json
  type: apiKey
slug: anytax-authentication
source_filename: anytax-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/anytax-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/anytax-openapi.json\n- name: api-key\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key for programmatic authentication\n  sources:\n  - openapi/anytax-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/anytax/authentication/anytax-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Fintech
- Tax
- Integration
- Banking
- Tax Planning
- White Label
- Compliance
---
