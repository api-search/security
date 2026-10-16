---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: bestprintondemand-account-api-openapi.yml
  format: yaml
  label: BestPrintOnDemand Account API
  slug: bestprintondemand-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bestprintondemand/refs/heads/main/openapi/bestprintondemand-account-api-openapi.yml
- filename: bestprintondemand-batches-api-openapi.yml
  format: yaml
  label: BestPrintOnDemand Batches API
  slug: bestprintondemand-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bestprintondemand/refs/heads/main/openapi/bestprintondemand-batches-api-openapi.yml
- filename: bestprintondemand-gender-api-openapi.yml
  format: yaml
  label: BestPrintOnDemand Gender API
  slug: bestprintondemand-gender-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bestprintondemand/refs/heads/main/openapi/bestprintondemand-gender-api-openapi.yml
- filename: bestprintondemand-webhooks-api-openapi.yml
  format: yaml
  label: BestPrintOnDemand Webhooks API
  slug: bestprintondemand-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bestprintondemand/refs/heads/main/openapi/bestprintondemand-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Bestprintondemand Authentication
name_suffix: Authentication
oauth_flows: []
overview: BestPrintOnDemand secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: BestPrintOnDemand
provider_slug: bestprintondemand
scheme_count: 2
schemes:
- description: 'Recommended: `Authorization: Bearer <key>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/bestprintondemand-openapi.json
  type: http
- description: Alternative header form, for clients that cannot set `Authorization`. Keys are never read from the query string or the request body.
  in: header
  name: apiKeyHeader
  parameter: X-Api-Key
  sources:
  - openapi/bestprintondemand-openapi.json
  type: apiKey
slug: bestprintondemand-authentication
source_filename: bestprintondemand-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: derived\nsource: openapi/bestprintondemand-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Recommended: `Authorization: Bearer <key>`.'\n  sources:\n  - openapi/bestprintondemand-openapi.json\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: Alternative header form, for clients that cannot set `Authorization`. Keys are\n    never read from the query string or the request body.\n  sources:\n  - openapi/bestprintondemand-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bestprintondemand/refs/heads/main/authentication/bestprintondemand-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- API
- Print-on-Demand
- Pricing
- OpenAPI
---
