---
anonymous_access: false
api_key_in: []
api_specs:
- filename: datocapital-com-account-api-openapi.yml
  format: yaml
  label: Dato Capital Account API
  slug: datocapital-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datocapital-com/openapi/datocapital-com-account-api-openapi.yml
- filename: datocapital-com-companies-api-openapi.yml
  format: yaml
  label: Dato Capital Companies API
  slug: datocapital-com-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datocapital-com/openapi/datocapital-com-companies-api-openapi.yml
- filename: datocapital-com-filings-api-openapi.yml
  format: yaml
  label: Dato Capital Filings API
  slug: datocapital-com-filings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datocapital-com/openapi/datocapital-com-filings-api-openapi.yml
- filename: datocapital-com-health-api-openapi.yml
  format: yaml
  label: Dato Capital Health API
  slug: datocapital-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datocapital-com/openapi/datocapital-com-health-api-openapi.yml
- filename: datocapital-com-individuals-api-openapi.yml
  format: yaml
  label: Dato Capital Individuals API
  slug: datocapital-com-individuals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datocapital-com/openapi/datocapital-com-individuals-api-openapi.yml
- filename: datocapital-com-reference-api-openapi.yml
  format: yaml
  label: Dato Capital Reference API
  slug: datocapital-com-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datocapital-com/openapi/datocapital-com-reference-api-openapi.yml
- filename: datocapital-com-suggest-api-openapi.yml
  format: yaml
  label: Dato Capital Suggest API
  slug: datocapital-com-suggest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datocapital-com/openapi/datocapital-com-suggest-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Datocapital Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dato Capital declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Dato Capital
provider_slug: datocapital-com
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: All /v3 endpoints except /v3/health and /v3/ready require a bearer token.
  scheme: bearer
  type: http
slug: datocapital-com-authentication
source_filename: datocapital-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://api.datocapital.com/docs/authentication\nschemes:\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: \"All /v3 endpoints except /v3/health and /v3/ready require a bearer token.\"\n"
source_yaml_url: https://artifacts.apis.io/datocapital-com/authentication/datocapital-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Data
- Search
- Compliance
- Due Diligence
---
