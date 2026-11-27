---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: nobounceapi-com-domain-api-openapi.yml
  format: yaml
  label: NoBounce Domain API
  slug: nobounceapi-com-domain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nobounceapi-com/openapi/nobounceapi-com-domain-api-openapi.yml
- filename: nobounceapi-com-find-email-api-openapi.yml
  format: yaml
  label: NoBounce Find Email API
  slug: nobounceapi-com-find-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nobounceapi-com/openapi/nobounceapi-com-find-email-api-openapi.yml
- filename: nobounceapi-com-health-api-openapi.yml
  format: yaml
  label: NoBounce Health API
  slug: nobounceapi-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nobounceapi-com/openapi/nobounceapi-com-health-api-openapi.yml
- filename: nobounceapi-com-validate-api-openapi.yml
  format: yaml
  label: NoBounce Validate API
  slug: nobounceapi-com-validate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nobounceapi-com/openapi/nobounceapi-com-validate-api-openapi.yml
- filename: nobounceapi-com-validate-bulk-api-openapi.yml
  format: yaml
  label: NoBounce Validate Bulk API
  slug: nobounceapi-com-validate-bulk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nobounceapi-com/openapi/nobounceapi-com-validate-bulk-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: NoBounce Authentication
name_suffix: Authentication
oauth_flows: []
overview: NoBounce secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: NoBounce
provider_slug: nobounceapi-com
scheme_count: 2
schemes:
- description: Your NoBounce API Key (e.g. nb-xxxx...) or RapidAPI key
  in: header
  name: ApiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/nobounceapi-com-openapi.yml
  type: apiKey
- description: Your NoBounce API Key passed as a query parameter
  in: query
  name: ApiKeyQuery
  parameter: api_key
  sources:
  - openapi/nobounceapi-com-openapi.yml
  type: apiKey
slug: nobounceapi-com-authentication
source_filename: nobounceapi-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/nobounceapi-com-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Your NoBounce API Key (e.g. nb-xxxx...) or RapidAPI key\n  sources:\n  - openapi/nobounceapi-com-openapi.yml\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Your NoBounce API Key passed as a query parameter\n  sources:\n  - openapi/nobounceapi-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/nobounceapi-com/authentication/nobounceapi-com-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Email Verification
- Automation
- Data Validation
- Software-as-a-Service
---
