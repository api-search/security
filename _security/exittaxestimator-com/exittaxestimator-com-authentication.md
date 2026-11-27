---
anonymous_access: false
api_key_in: []
api_specs:
- filename: exittaxestimator-com-enquiry-api-openapi.yml
  format: yaml
  label: Exit Tax Estimator Enquiry API
  slug: exittaxestimator-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exittaxestimator-com/openapi/exittaxestimator-com-enquiry-api-openapi.yml
- filename: exittaxestimator-com-guide-api-openapi.yml
  format: yaml
  label: Exit Tax Estimator Guide API
  slug: exittaxestimator-com-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exittaxestimator-com/openapi/exittaxestimator-com-guide-api-openapi.yml
- filename: exittaxestimator-com-mcp-api-openapi.yml
  format: yaml
  label: Exit Tax Estimator MCP API
  slug: exittaxestimator-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exittaxestimator-com/openapi/exittaxestimator-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Exit Tax Estimator Authentication
name_suffix: Authentication
oauth_flows: []
overview: Exit Tax Estimator secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Exit Tax Estimator
provider_slug: exittaxestimator-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/exittaxestimator-com-openapi.json
  type: http
slug: exittaxestimator-com-authentication
source_filename: exittaxestimator-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/exittaxestimator-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/exittaxestimator-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/exittaxestimator-com/authentication/exittaxestimator-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Tax
- Illinois
- ExitTax
- Finance
---
